# How Did MP3.com Play MP3s?
## April 4, 2020
### From gopher.somnolescent.net, the Gopherhole of the weird lightbulb people
Through their archived help documents, we can answer this question.

---

As you might know if you regularly read the Scratchpad, I was fascinated
with MP3.com. And really, I still am. The more I learn about it, the more I
realize that it was *the* first great cultural equalizer, one the internet
was always capable of, the first time in history garage bands across the
street shared shelf space with bands as big as the Eagles, Linkin Park, and
Tom Petty. It seems passe in the age of Bandcamp, but I think of MP3.com as
a literal digital Atlantis, a sunken city all but forgotten, unfortunately.

And another piece of the puzzle has since fallen: how music actually worked
on the site.

We're a spoilt bunch, here in the comfort of modernity. Audio is directly
playable in the browser through a variety of quick, pleasant methods, but in
2000, some assembly was required. Modern browsers have players built-in, and
if they don't, every computer comes with some basic freebie MP3 player on
board, some quite capable as fully-fledged digital jukeboxes (in the case of
iTunes/Apple Music and the former Windows Media Player). In 2000 though, the
situation was a lot more discombobulated. Setups varied wildly across even
computers running the same OS. The internet made interoperability a pain.

As a result, the answer to the question "how did MP3.com actually play MP3s?"
isn't so obvious. When I wrote my initial MP3.com posts, I wasn't even sure
MP3.com streamed *using* MP3! All I knew was that music streamed through some
kinda CGI script, but whether that meant a player in the browser, a
redirector, or some other 90s oddity, it was hard to tell.

Anyway, now I know, and here's the setup. Hope you like technical
explanations!

This all starts with an identifier known as a MIME type. MIME types are a
quick way to let the browser know what the file it's trying to download is,
exactly. We might think file formats are relatively cut and dry, but not
quite. To a computer, data is data. It can guess based on the file extension,
but that only goes so far. Classic Mac OS and Unix didn't use file extensions
back then. Magic numbers might work, might not. In 1996, in a world where
Windows 9x, NT, Classic Mac OS, Solaris, BSD, and Linux were all
intermingling, getting them all on the same page was a shitshow that MIME
types were meant to solve.

*Everything* accessible online has a MIME type; when you download a file, the
server sends the MIME type in the HTTP header, and hopefully, the browser
will know what to do with it, prompting the user if not. **This is the key
bit:** what happens next *isn't* standardized. It's up to the browser to
handle the file however it will.

So getting back to MP3s, when the browser encounters the `audio/mpeg` MIME
type, a Mac could open that in Quicktime, while a Windows machine could open
it in Winamp or RealPlayer or whatever else the user had MP3s set to open in.
This kept everyone happy and on the same page, though it naturally
necessitated a bit of setup, as can be seen in some of MP3.com's archived
help documents.

This is also where plugins came into play: if the browser detected a MIME
type of `application/vnd.adobe.flash-movie` (for Flash games and animations),
and Flash Player wasn't installed, the browser would report an unknown MIME
type and the site in question would direct people to download the plugin
needed to see the file. If Flash Player was installed, the browser would
recognize the MIME and forward the SWF to the player to handle it instead.

So getting back to MP3.com specifically. While scouring their help pages for
any information on how their CGI script worked, I came across this bit:

> **How do I stream ("HiFi"/ "LoFi") MP3 files from MP3.com using my
> MusicMatch player?**
> 
> You need to have high-speed Internet access (cable modem or better) to
> take advantage of the "HiFi" feature. For all other internet connections
> click "LoFi".
> 
> If you have downloaded MusicMatch from this site, or you have version 4.1
> or higher of the player, click on either "HiFi" or "LoFi". This should
> automatically launch your MusicMatch player. If this doesn't happen, go to
> the menu bar on your MusicMatch player, click on "Options," and scroll down
> to "Settings." Make sure that all boxes by the "Add to Music Library" and
> "Add to Play List" prompts are checked. If you're still having problems,
> you may need to try configuring your browser.

Open and shut case! MP3.com's CGI script wasn't a player in the browser like
I was guessing, but rather, a forwarder for an external program, in this case
MusicMatch Jukebox. MusicMatch is perhaps best covered by dcb, but in short,
it was a rather common MP3 player, ripper, audio recorder (!), and library
manager at the time, pushed pretty heavily as bloatware packed in with
people's Packard Bells and whatever else. MP3.com loved MusicMatch, likely
because they got paid to promote it.

This is also the difference between the "download" and "lo-fi/hi-fi play"
options. MP3s can be loaded in in one of two ways, either directly as MP3s or
through special playlist files with the M3U extension. These are pretty
standard: web radio uses them. While MP3s have the `audio/mpeg` MIME type,
M3U has...well, no standardized MIME type at all, though a couple were
commonly used: MP3.com used `audio/x-mpegurl`.

The major difference between an MP3 and an M3U in practice was that M3U
files are streamed, while downloaded MP3s are loaded and played in one go.
This makes all the difference over dial-up connections; if you were to
download a 128kbps MP3, under the most optimal of 56k conditions, you'd still
be waiting about ten minutes for your song. Streamed, though, you could
listen as the file is downloaded.

So at long last, here's how I think MP3.com worked in practice:

- Users uploaded MP3s to the service. I can't find any documentation on this,
but likely, they were required to be at 128kbps. Naturally, sound quality
could differ depending on the encoder used and competency of the band.
MP3.com automatically generated 24kbps versions of those for low quality
streaming.
- All download links went through a CGI forwarder that would send the
relevant file to the client computer's browser, who'd then choose what to do
with it based on the MIME type received.
  - If the "download" option was picked, MP3.com would send the
  "high quality" 128kbps version of the file in full for local playback.
  - If "lo-fi play" was picked, MP3.com would send an M3U to the client
  containing a pointer to the low quality 24kbps version of the song on their
  servers, where MusicMatch or some other software would stream it direct,
  being much faster than downloading it.
  - If "hi-fi play" was picked, the same would happen, but the M3U would
  point towards the high quality 128kbps version of the file.

This pretty much settles the last of my curiosity with MP3.com, at least on
the user experience. Certainly an experience compared to just having a neat
little player on the page itself like you do these days.

At any point during this little expedition, you might've been inclined to ask
why I care about the details so much, why I want to know all these gory inner
workings of a long-forgotten music streaming site. And aside from the
obvious, easy answer involving a certain mild mental disorder I have, I'd say
I do it for the sake of documentation, curiosity, and potential, hazy future
plans of mine.

Which is a funny way of saying I'm probably gonna clone MP3.com for funsies
someday.