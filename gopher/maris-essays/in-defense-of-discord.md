# In Defense of Discord
## October 2018
### From gopher.somnolescent.net, the Gopherhole of the weird lightbulb people
Let's put this nonsense to bed, because it's cranky and needs a nap. Discord
is not malware.

---

*Throughout this piece, I'll be referring to the Discord privacy policy,
which is as legally binding as you can get without signing anything. You
agree to this the moment you make your account, and if you don't agree to the
privacy policy, you don't have a right to use the service. Read it for once.
I had a piece I was using as the base for my rant, but the user deleted their
account before I could post this. The piece is still quoted extensively
throughout. I'll also be quoting from the Spyware Watchdog site, which I'm
much less charitable towards because it reads like a smug schizo's tinfoil
dream.*

Discord skews young. I imagine if you took metrics on Discord's active users,
the average user age would probably sit somewhere in the early twenties. I'm
sure, as anyone who's seen a callout post can cop to, young people aren't
really the smartest when it comes to rallying and getting on the horn for a
cause.

Now, I happen to love Discord. It's the best of all worlds: convenient,
everyone's in one place, works well, good interface, free (and I hope to buy
Nitro at some point in the future), and has a ton of nicer, smaller features.
After bouncing between Skype and IRC for years, with neither really
satisfying, Discord has been just the thing my little circle of friends
needed.

But, every so often, some jumped-up well-to-do from the woke computer kids
crowd will pop up, usually on a site like Neocities, and talk about how truly
awful Discord is. "Guys," they'll say, with a thousand-yard stare, their
voice quivering. "It's literally malware."

> Discord can track your general location (about as precise as which county
> you are in). Discord can also tell which devices you use, as it uniquely
> identifies each device, and how much you use those devices, as it can
> record your device usage habits (since Discord is usually open in the
> background so that it can receive messages). Discord also records every
> single interaction you have with other users through its service. This
> means that Discord is confirmed to log every conversation that you have
> through Discord, and record everything that you say on Discord, and view
> all images that you send through Discord. Therefore, none of your
> interactions on Discord are private.

Gee, thanks, my guy. I didn't realize an app I use for chatting with other
people meant other people were gonna see what I sent.

My ire this time rests on a piece from a new Neocities user, who sarcasm
aside, I'm sure is actually fine. Unresearched, hyperbolic scaremongering
doesn't sit well with me though, and that's what I'll focus on for the rest
of this rant. Everything is sourced either from the Discord privacy policy
or material on their Reddit written by employees. It's all a Google search
away, or DuckDuckGo, or whatever the woke computer kids crowd is using this
week. Please use it.

> Discord, by design, gathers data. Whether or not that data is of value to
> you as the user with full knowledge that the data gathered can (and will
> be) used to market third-party services to you is important, is your call.
> Assuming most Neocities users are cautious of privacy and advocate free
> speech, this is an oxymoron. Discord is a messaging service, a space for
> gamers, creatives, and other users to talk and share information. Having
> prying eyes for every sentence you mention (for example) in a vent channel
> with a space to converse about feelings and otherwise troubling situations,
> is completely open for third-parties to sell you medications and suggested
> psychological evaluations.

Malware is defined by Wikipedia as "any software intentionally designed to
cause damage to a computer, server or computer network". Malware takes many
forms, but most often, the term refers to viruses, worms, trojans,
ransomware, adware, and spyware, the latter of which is generally what people
classify Discord as being. After all, Discord collects your data, spyware
collects your data, literally what's the difference?

The major issue with spyware isn't the tracking, but rather, the opaqueness
of how your data is used. If you send your phone number through a spyware
app, that app now has carte blanche to sell it off to anyone looking to spam
you with advertisements or order pizzas on your behalf.

Discord, on the other hand, is very open about how it collects and uses user
data, with a section dedicated to it in their privacy policy:

> If you provide information for a certain reason, we may use the information
> in connection with the reason for which it was provided. For instance, if
> you contact us by email, we will use the information you provide to answer
> your question or resolve your problem. Also, if you provide information in
> order to obtain access to the Services, we will use your information to
> provide you with access to such services and to monitor your use of such
> services. The Company and its subsidiaries and affiliates (the "Related
> Companies") may also use your information collected through the Services
> to help us improve the content and functionality of the Services, to better
> understand our users and to improve the Services. The Company and its
> affiliates may use this information to contact you in the future to tell
> you about services we believe will be of interest to you. If we do so, each
> marketing communication we send you will contain instructions permitting
> you to "opt-out" of receiving future marketing communications. In addition,
> if at any time you wish not to receive any future marketing communications
> or you wish to have your name deleted from our mailing lists, please
> contact us as indicated below.

tl;dr Discord uses your data to provide you the service, improve the service,
and to market stuff it thinks it likes to you. If you don't like the latter,
you can opt out of the latter. If you don't like it using your data at all,
*you can stop using the service*.

Discord makes it very clear, in both official Reddit posts and in their
privacy policy, that they **do not sell user data to advertisers**. The data
they collect doesn't leave the station. Discord *does* reserve the right to
aggregate information, but this is much less specific data, mostly
demographics. In short, they're not marketing to you, sit down.

So yeah, this is pretty much a fool's understanding of how spyware works.
It's disingenuous to say that a free program that tracks your data openly to
make the service work is in the same class as, say, CoolWebSearch, or apps
masquerading as Netflix. Also, **Discord doesn't sell data to advertisers.**

Further, I'm not sure what privacy you expected on Discord, a place where any
little shit with a copy of ShareX can leak a server's worth of embarrassing
messages to any parties interested. I'd be more scared of them than the
spooky monolith gamer chat people that, no, do not care about your furry kink
and aren't trying to sell it to advertisers. Perhaps you could just, I dunno,
crazy idea, don't jump at me for saying this--not send private information
through Discord?

> Also running is Discord's process logger and web cookie sniffer to
> parasitically attach itself to every account you ever logged in with in
> your preferred web browser.

This fucking "process logger" nonsense, I swear. This seems to be something
of a smoking gun for the woke computer kids crowd, *true evidence* of
Discord being malware...until you read further into it:

> CTO of Discord here.
> 
> We do not record all your processes and send them to our servers.
> 
> We watch the process list for 3 reasons.
> - Detect games to show on your status message. You can turn this off
> anytime in the privacy tab of settings.
> - Detect games to hook the overlay into if it is enabled.
> - Detect games run as administrator to warn that Push to talk won't work.
> You cannot disable the scanning as the 3rd reason is always required.
> 
> If you use the overlay we send information about your DirectX and GPU to
> our metrics server to track success rate of the overlay as we test it and
> improve it. We will probably stop sending this to our server as soon as
> overlay moves out of the experimental phase.
> 
> Nothing else is ever saved to disk or sent over the network.

Astoundingly, this is cited on the Spyware Watchdog site as a *confirmation*
of spying, which kinda makes me wanna scream.

I take umbrage with the term "cookie sniffer" as well. In short, Discord used
cookies, small chunks of data stored in your browser to remember pertinent
information, to track notifications and login states. Discord uses Google
Analytics, which also uses cookies.

No other site *in the history of the world* (probably) has used cookies. The
ones that do are (probably) evil and fascist and (probably) look to bring
about nuclear armageddon using small Filipino children to carry dirty,
radioactive bombs into the Capitol Building. How eeeeeeeevil.

> Truth is, there is no seperation between the user's messages and the
> profit-value us Neocities users are formally against.

Speak for yourself.

> Written in Electron and Node.js, which means Discord is a self-contained
> Chrome-based browser simply acting as a portal to the web version of
> Discord. In multiple occasions, Discord ramps from the standard 90MB of RAM
> usage to nearly 1GB. Not forgetting the RAM leaks due to Electron's bloated
> mess (Tested on an i5-6600 + 16GB RAM). All for a messaging app.

This is a side point I'd like to address. Electron is actual trash, but
Discord is actually one of the best Electron apps I've used. I know, that's
like saying you're the fastest runner in the Paralympics, but stick with me.
For a while, I used Trello's desktop app, which also uses Electron, and the
damn thing was responsible for grinding my computer to a fucking halt
constantly. Meanwhile, I have Discord running on both machines 24/7 with
virtually no system slowdown whatsoever, even during gaming and recording, on
the same processor and *less* RAM.

Where's your God now?

> Marketed as a simple messaging app, when really bundled as malware.

Like clockwork. Pray the knees stop jerking.