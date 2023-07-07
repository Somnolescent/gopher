# Recap #10: Underground, Dig Holes, Plant Seeds, Grow Old
## May 30, 2020
### From gopher.somnolescent.net, the Gopherhole of the weird lightbulb people
You feel that? That sunshine on your shoulders and that crisp, clean air in
your lungs? That's spring in full bloom, my friend, and that means *flowers*!
Flowers, gardening, growing season, chamomile--wait, what the fuck dug all
these holes?

---

## Gopher returns!
In this month's headline news: Gopher! No, not the burrowing rodent, the old
protocol, and more specifically, Somnolescent's Gopher server! It's a long
story, but in the early 90s, between FTP servers getting people their
industrial music fix and Telnet connecting nerds to MUDs, Gopher promised
colleges what the World Wide Web would eventually deliver. At least, that's
the line, isn't it? Really, Web comparisons do both the Gopher and the Web a
disservice, so Somnolescent started a camp in both.

About a year ago, technical issues knocked our Gopher offline, and sometime
in March, we decided that enough was enough and that the Gopher would rise
from its grave come May. And here we are! The server (running Pituophis, our
in-house server software courtesy of dcb) has been totally reorganized by
project rather than user, which lets us to share all these fun odds and ends
for them that just don't fit anywhere else. So hey, if 8-bit/11khz WAVs,
crunchy GIFs, and text files appeal to you as much as they appeal to us,
you'll feel right at home.

The Gopher's homed where it was at gopher.somnolescent.net. I'd tell you how
to get there right here, but you're already reading this on Gopher! Good
taste you have.

## The Gopher Information Repository returns!
And right alongside the Gopher itself, my Gopher Information Repository gets
a tuneup. I unveiled that thing early last year, only for it to lie dormant
and embarrass me ever since. At long last, with dcb's help, I've brought it
up to speed with a ton of new content and some light styling. Still nowhere
near complete (there's still clients to review!), but this is infinitely
superior to what was up before, I promise you.

## Pituophis returns! (with a friend!)
As mentioned previously, Somnolescent's Gopher is running on dcb's
Pituophis, which is more accurately a Gopher client/server library written in
Python. I was adamant about using it, given the work he's put into it and
that it's cool to say we're running our own software, but what I didn't
expect was for dcb to write a damn *search function* to integrate in it.

A little project of his I admittedly didn't pay much attention to at first
was Gophew, which is a Gopher crawler and search engine. The traditional
Gopher search engine is Veronica, which is essentially a cursory metadata
search across all of Gopherspace. There's also Jugtail, which is per-server
and a bit more in-depth, but the question of how we'd integrate either into
our setup was up in the air.

dcb being the powerful little bastard he is, he took option three and
rewrote Gophew to run over top Pituophis. In one script, we have Pituophis
serving Gopherhole requests and Gophew intercepting search requests, letting
people scan through our entire server from a single selector.

## Gopherlens...returns?
In addition to the server itself, Somnolescent now runs its own Gopher proxy
service on gopherlens.somnolescent.net. Originally, Gopherlens was just a
repl.it project powered by Pituophis, but after the Gopher server went up,
dcb suggested making it an official part of the setup. I wasn't able to get
it working on the Pi itself, but DreamHost offers Python through Passenger,
which has worked out well enough for being a tower of duct tape.

I'd personally still recommend a separate client, but in a pinch, Gopherlens
works, and I'd say works better than Floodgap's proxy, especially given the
latter rendering our menus incorrectly at the moment.

## Somnocraft definitely does not return
In an old Letters post I made called "Somnoville", I said this:

> I can't really show off everything in a blog post, obviously, but I'll have
> a page up on the main Somnolescent site showing off everything sometime
> this month.

Well, it wasn't that month, it was about ten months later, but I finally
finished off the Somnoville page, showing off all the builds from our group's
first shared private *Minecraft* server. We stopped playing that world
sometime around August, and the page was similarly left half-finished.
Wasn't really fair, given all the effort we pumped into it, so on some off-
time, I finished it up and Caby and mon helped with the rambles.

(I don't really consider it worth its own section, but while we're talking
old work made new again, I also dug up and recreated the first ever site
design I had on my subdomain. I didn't save the original files, but Caby and
the Wayback Machine saved a few, so I did what I could to piece together the
rest. Kinda nice to see it back again, in all honesty.)

## Blog highlights
Comparatively less happened on the blog front this month, but still worth
mentioning:

- Tools, Toys, and You and I by mariteaux (May 9): "Technology should augment
what we already naturally do and open up our world, not replace our old way
of being."
- Somnolescent Radio: Spring 2020 by everyone (May 17): "As the first one
went, each Somnolian has chosen a song dear to them at the moment and written
a bit about it. Have a listen."
- Incomplete Eclipses and Muffled Screams by borb (May 22): "Was on this site
for 6 years and I'm pretty sad to see it crash and burn like a drunk teenager
driving their mom's car, but that's just the moral of this story. Get too
cocky and forceful and suddenly everyone's mad and one is spamming yiff porn
at you."

Gosh, busy, busy. I'm never using the word "Gopher" again...unless it's in
reference to Pennyverse! But that'll have to wait for next month. Keep cool,
my friends.