# On Website Restoration
## September 2nd, 2020
### From gopher.somnolescent.net, the Gopherhole of the weird lightbulb people
A rare philosophical ramble from me!

---

So happy September, lads. Sudden major mood boost last night and now I'm
500something words into a new story for Pinede. Pretty stoked.

I don't really do the unsolicited opinion posts anymore, not unless something
sets it off and not unless it's something I feel someone could potentially
have a discussion with me on. Course, it being my Scratchpad and the biggest
fan of the Scratchpad being me, who am I to disappoint? So given that it's
not quite bedtime and yet a bit too late to get cracking on anything heavy
(trying not to stay up into the wee small hours of the night anymore), here's
something I've been thinking about lately: website mirrors and what level of
restoration is worthwhile from a preservation standpoint.

Yesterday's post was on the restoration of an old website called The Forge.
I got my working copy from someone else's mirror, though the mirror seems to
otherwise unaltered from the Wayback Machine's copy, so I'm fairly certain
it's accurate as far as source goes. Still, as with most old sites, The Forge
doesn't look quite right on modern monitors, and it's to do with width.

Back in 1997, 800×600 was considered a high-res desktop resolution, and sites
were still being commonly built for 640px. The Forge sets its tables to two
widths, generally: 600px, which still looks fine of course, and 90%, which
doesn't. At the time, 90% of 800px would've been a comfortable reading
experience with margins on both sides, given that it's centered; now, it's
just way too wide, proving both irritating to read and inaccurate to how the
site would've been viewed in 1997.

This raises an interesting question: what is "accurate" as far as web pages
go? Is it uncompromised markup with rendering errors on the viewer's end, or
is it inaccurate markup with widths constrained to more period-appropriate
(not to mention more comfortable) values? I lean towards the latter. The
intended experience is the finished site loaded in the browser as a layout,
text, and images, not as a page of unrendered markup. Thus, while a
constrained width is inaccurate, the viewing experience is better and closer
to what was intended.

Of course, things will never be completely accurate because web pages are not
an absolute canvas. Pages will render completely differently on different
generations of browsers, both newer and older than the contemporary ones. Even
contemporary ones differ: if Internet Explorer renders its inline audio
players in such a way that the layout ends up warped, it's certainly visually
inaccurate even though the same source page is being rendered. There's too
many variables at play, too much error from too many humans, to say anything
is exact. Total accuracy will never be achieved because there never was a
completely accurate way to look at this site.

Of course, a true preservationist would probably say any edits at all to the
source material compromise the integrity of it. While I'd agree, I'd also put
forth the following point: the Wayback Machine, formerly the gold standard of
archival sites before it fell to political mischief, does not perfectly
preserve pages. Look at the page source of anything it's saved: it adds
tracking scripts and explicitly modifies the page's visuals to messily insert
the toolbar it uses for navigation. Even if this is simply a server-side
runtime script and the original pages are perfectly preserved, to the viewer,
the page has been compromised.

What is the difference between the Wayback Machine doing this and a human
doing this? Both humans are robots are capable of malevolently editing pages,
if that's the concern. If anything, robots are capable of far more damage.
Even saving a page to your computer as "complete" changes the links to refer
to the local copy and not the ones online. Nothing perfectly preserves site
markup. Therefore, I say it's fair game.

I did go a little further than that, however. Given that my operating
assumption is that the intent of the site developer is what matters and not
what's actually on the page, I fixed a variety of bugs in the original site's
markup. Some involved the layout of the page itself; if you look at the March
1998 news page on the original mirror, you can see it's really broken. I
straightened it out a little on my mirror. Any scripts and ads relating to
GameSpy got removed (because they don't work anyway anymore). Broken esoteric
symbols got patched, as the original site didn't specify character encoding
and the mirror therefore saved wrong. I also ran HTML-Tidy over many of the
pages I didn't patch by hand, and those I did, I practically rewrote by hand
to make them as readable as possible.

Now, the one area I do draw the line in is rewriting pages that originally
didn't use stylesheets to use them. Back when The Forge was written,
stylesheet support was nonexistent or just barely supported in some browsers;
thus, it doesn't use one. Since using a stylesheet would therefore compromise
how the page renders on these older browsers (and again, I'm going off intent
and visual accuracy), I opted not to add one. This also extends to the many
links on the site that use JavaScript to set the status bar; modern browsers
ignore it and simply display the link URL instead. Minor detail, but given
that older browsers obviously still support it (plus browsers forked from
their code, like RetroZilla), I left it in.

I think there'd be a lot of people who would ask me what point there is in
restoring an old website that not even the people behind it have thought
about in 20 years. To be perfectly honest, I don't really have a point. It's
really just something that pleases me. That said, the one place I can
objectively justify a site restoration is when content's been lost or gone
missing from a mirror. My entire reason for doing this was that The Forge's
file downloads were never stored with the site itself, and while they
thankfully survived, they weren't in their proper context on an FTP server.
Merging the two only makes sense.

And since I was already working on that, I figured I might as well clean the
visuals up as a labor of love...

...and that's how you end up with a mirror like mine. It's a curiosity, one
of a few on my radar. If they'll get the same love and care or if I'll just
run Tidy over them, I'll have to see. Point or not, it's nice to bring little
historical relics like this back from the brink, and like VDU itself, the
content's safe with me now. I'm sure at least someone in the old web crowd
would appreciate it.