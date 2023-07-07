# 320kbps (and Other Lossy Audio Voodoo)
## September 21st, 2020
### From gopher.somnolescent.net, the Gopherhole of the weird lightbulb people
I’m basically convinced no one on the internet understands how lossy audio
works.

---

I handle MP3s on a pretty regular basis. I have my own vaguely picky
specifications for how I want my music collection, neatly sorted in lossless
for later use in fucking around (or in the original format and bitrate if
lossy to begin with), but I keep a set of casual listening MP3s on this
computer and the eMachines box and they do well enough.

In all my handling, I've also come across some serious sophistry. I think
anyone into this hobby has. Consumer audio is basically the premiere avenue
for snake oil today, thanks to the fact that our ears are shit and easily
biased by perception. You throw enough money at this hobby, enough gold-
plated cables and vacuum tubes, and you too can become an armchair engineer,
casually able to pick out the *slight distortion and sibilance in the high
frequencies* with the best of them.

Naturally, there's a lot of misconceptions people have about audio,
especially lossy audio (you know, MP3, AAC, Opus, Vorbis), and they irritated
me enough to rant a bit about them. Keep in mind, I didn't go to school for
this, I'm just an asshole on the internet, so for all I know, we all really
do need to listen to our MP3s through high-bias 24-bit fiber-optic
supergrounded kosher DACs. Somehow, I doubt it.

## "I can tell between two high bitrate formats with my $25,000 audio setup"

This is something I see said a lot on various audio forums–basically, some
lifelong audio geek has a completely overkill setup and can tell the
difference between a compressed bit of audio and an uncompressed one,
therefore he's really cool and MP3s are stinky.

I think the internet has totally forgotten the role that lossy audio was
meant to play. It's lossy; by its nature, using a lossy audio codec means it
will sound worse. Whether or not you can tell the difference is irrelevant.
The reason you do this is to make the file small enough that people can
handle them freely on bad computers and slow networks. These are not
audiophile formats and they were never meant to be.

When MP3s first appeared in the mid-90s, the CD (itself considered a
perversion of good quality audio for a time) was the gold standard of audio
reproduction. There is no compression involved with Red Book CD audio. For
all intents and purposes, it is as good as you'd ever conceivably want.
(Some people have tried to force the "HD audio" meme which involves higher
sampling rates that we can't hear and a higher bit depth that we also can't
hear; needless to say, DVD-A and SACD never took off for a good reason.)
You weren't meant to listen to MP3s all day; you were meant to use them when
you couldn't listen to your CDs.

In any event, whether or not they can genuinely hear a difference is kind of
irrelevant, because you're not meant to listen to MP3s on the kinds of setups
that could conceivably poke holes in the format. They're meant for
broadcasting over the radio, or over the internet, or for use in little
portable players where you're probably too busy listening to train and car
noises to care much about some wonkiness in the high frequencies. If you have
a good setup, good! Keep going with lossless. *That's what they're meant for.*

Of course, I kinda doubt these people really *can* tell a difference anyway.
To date, no one has provided ABX results that show they can reliably tell the
difference between, say, -V0 MP3 and an uncompressed original. With increases
in encoder tuning and efficiency, Lame 3.100 actually does fairly well (as
in, not annoying, not as in it's transparent) at 128kbps, let alone higher
up. A lot of these threads are dated 2002, 2003, and I'm sure with a modern
encoder and the right format (like AAC or Opus), these guys wouldn't have a
clue.

Of course, these people would then say something to the effect of "well,
ABXing is useless anyway because it's like 15 seconds of each, I've been
listening to these songs for years and I know how they're supposed to sound."
Yes, real post on one of these forums! And at that point, kids, you just give
up and start drinking.

## "If I convert it to a higher bitrate MP3, it'll sound better"
To repeat from the last section: lossy is lossy. You will never get the
original data back unless you start from the lossless file again.

Converting between compression formats is called *transcoding*, and lossy-to-
lossy (or lossy-to-lossless-to-lossy, I'll come back to that) is a
ridiculously bad idea. The algorithms involved are meant to work on
uncompressed audio. Of course, they'll work on any audio, but the way these
things throw out information means it's infinitely more likely to make the
existing compression artifacts even worse. Doesn't matter the bitrate,
doesn't matter the format (except AAC-to-AAC, for some reason, those tend to
be okay on transcode); it's a bad idea.

I've seen one too many very bad sounding MP3s that are, ostensibly, 320kbps,
and I know someone got cheeky somewhere down the road, took what's probably
128kbps, and converted it to 320kbps. This happens a lot with stuff you
download from file-sharing networks or strange Blogspots. Believe it or not,
even going up to the format's maximum bitrate, you'll *still* make the file
slightly worse sounding (not to mention much bigger for no improvement,
thanks) by re-encoding. The damage is just likely to be more slight thanks to
the higher bitrate.

I know there are fair reasons to transcode, like if you wanted to put a
Vorbis file on an iPod, but trying to get better sound quality from an MP3 by
re-encoding the MP3 is not one of them. Seek out a lossless or uncompressed
copy and use the format and bitrate that you want to use from the start.

## "If I convert it to FLAC, it'll sound better"
So you might be even cheekier and think "well, what if I just convert this
MP3 to a lossless format? That'll get the loss back!"

Nope. It's still the MP3, just now incredibly bloated with no improvement in
sound quality whatsoever. It just won't lose any *additional* sound quality.
The original MP3 will always be the best it'll sound, and if you want to
convert it back to a lossy format, you'll be transcoding lossy-to-lossy in
essence.

This one especially gets to me because of how much larger FLACs are compared
to MP3s. If I want to get them small again, I have to transcode–and lose even
more quality in the process. Because Bandcamp requires a lossless upload,
I'll see people occasionally do this with their MP3s in order to get them on
the service. If you do this–please just include them in the download or offer
them zipped separately. I'll still happily buy the MP3s, I just don't want to
make them sound even messier.

The only time when storing lossy audio in lossless is a good idea is if
you're doing any kind of editing on it; storing it in lossless means you
won't lose any additional quality when you go back to edit it.

## "256kbps AAC is equivalent to 320kbps MP3" or suchlike
This is another bothersome bugaboo I see posted about sometimes, sometimes by
official site documentation even, albeit a more subtle one: the concept that
lossy formats are comparable enough that you can equate them at specific
bitrates.

AAC is different than MP3. Both are MPEG standards, sure, but AAC has an
additional 10-15 years of research behind it. AAC-LC is a leader down around
128kbps, and I'm convinced it's transparent at 192kbps, based on my ABXing
and ABXing I've had friends do. Both work completely differently, and when
they artifact, it sounds completely different. If you're using a non-
competitive MP3 encoder (like Xing) and a leading AAC encoder (like Apple
AAC), the chasm widens even greater.

It might sound pedantic, but it contributes this idea that lossy audio is
this simple, that one is equal to this one with these settings. They're
better for different things and format should be chosen based on your needs.
Don't care? I agree! Go with MP3 for everything unless you use Apple
products, then go with AAC. Otherwise, the best you'll get is that AAC is
transparent at a lower bitrate than MP3. Entirely different formats. It'd be
like saying a q50 WebP is equivalent to a q90 JPEG or something, you just
wouldn't say that.

For the record, 256kbps AAC is just as overkill as 320kbps, and I highly
doubt anyone can really, reliably hear the difference between either and an
uncompressed original. And speaking of that...

## "320kbps is/sounds the best"
This shit right here is why I wrote this post. I am so tired of seeing
320kbps MP3s. They're huge for no gain in quality, you can't transcode them
without fucking them up, and *everything*, from major labels packing in
download codes with vinyl to netlabels offering free downloads, give you one
choice in 320kbps MP3s.

Now, why the significance on 320kbps? You see, 320kbps is the reasonable
maximum bitrate you can have in an MP3. With a freeformat MP3, you can go
much higher, but no player will actually play those. 320kbps is about your
limit. Therefore, everyone's just said "okay, just encode everything at
320kbps! It'll sound the best, practically like the CD, and it'll work with
everything."

*No.*

As I said, 320kbps are a ridiculous waste of space for the fact that they
offer no benefit to sound quality over any of the higher bitrates, especially
in VBR. At that point, you're only getting about 20-25% space reduction over
a FLAC file of the same song, which loses *no* quality *and* can be
transcoded. Yet, for some ungodly reason, I don't get a FLAC download when I
buy an album on vinyl. I get a 320kbps MP3 download that both sounds no
better than -V0 or -V1 or even 256kbps and takes up more space on my device.

Now, I have had a friend who could (seemingly) reliably tell a 192kbps MP3
apart from the uncompressed original through ABX, but that was in CBR. In the
equivalent VBR mode (-V2), I doubt it'd be the same story. Certainly it
wasn't the same story with a 192kbps AAC file, which she got about half of
the trials right. 50% is no better than guessing. Therefore, I know it's
basically transparent at that bitrate, and my ears can't tell the 192kbps MP3
apart from the uncompressed, so I'm happy settling for that.

Again, this is the point of lossy audio: you find the lowest bitrate, and
therefore the smallest files, that doesn't offend your ears. If you're
looking to "maximize" quality, *use a lossless format*. Lossless formats are
mathematically identical to the CD, though much smaller, and give you the
option of converting to whatever bitrate and codec you need, with results as
good as that bitrate and codec will ever give you.

If you're bothered that streaming audio on SoundCloud sounds like shit, go
stream audio on your own fucking site, or better yet, sell CDs again! Not
like they weren't uncompressed from the start or anything...