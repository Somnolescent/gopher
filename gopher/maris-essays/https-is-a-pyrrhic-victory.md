# HTTPS is a Pyrrhic Victory
## July 23rd, 2020
### From gopher.somnolescent.net, the Gopherhole of the weird lightbulb people
When you’re online, you can be watched. No exceptions, no way around this.
Your padlock icon won't help.

---

So something I've talked about in a few Scratchpad posts to date, but haven't
really given the time to talking about it specifically, is HTTPS. HTTPS is the
secure version of HTTP, where page content is encrypted to myriad benefits.
You might know the song and dance there.

In my less contrarian moments, I don't think there's much actually wrong with
the use of HTTPS. In the scope of what it was meant to fix, HTTPS does work.
Your page and the contents of it get encrypted and no one tampers with your
stuff. Sounds great. It murders backwards compatibility with older browsers,
but who cares about those, who cares about supporting older hardware. We all
use new browsers, it's fine.

My issue is more with the constant obsession towards keeping a fundamentally
public medium private, trying to secure things that just can't be secured.
While we might appreciate the surface benefits towards encrypting our pages
(Comcast can't inject stuff into them, for one), none of that matters when
the rest of the chain is so paper thin and weak, and when, HTTPS or not,
people's data is still being systematically harvested, leaked, and exploited.
It's fine to celebrate a victory, just don't pretend like it means anything.

This starts when I was logging into *Letters from Somnolescent* and saw a
message from WordPress, telling me my site doesn't use HTTPS, with a "Learn
why you should use HTTPS" link underneath. Clicking that link takes you to a
WordPress.org support article extolling the virtues of HTTPS. It's fluff--
some of it's true, some of it's debatable, some of it's emotional--and kinda
manipulative fluff at that. The last bit of the article is what crawled up
my ass the furthest:

> **Your good name.** Have you noticed that some websites have the text
> "not secure" next to their address?
> 
> That happens when your web browser wants you to know a site is NOT using
> HTTPS. Browsers want you to think (rightly!) that site owners who can't be
> bothered using HTTPS (it's free in many cases) aren't worth your time and
> certainly not your money.
> 
> In turn, you don't want browsers suggesting you might be that kind of shady
> site owner yourself.

The sentiment that only idiots and bad people use HTTP is one that's fairly
common among these "why HTTPS is so great" pieces, and one I generally don't
like. HTTPS has some benefits, and thus people push for its use. This turns
into manipulation ("Google will demote you, everyone's doing it, and you
don't want people to think you're shady and dangerous, do you?") and then
outright fearmongering on the part of browsers by flashing a big "NOT SECURE"
sign up top any time you visit one of those spooky HTTP sites.

Problem is, this is a false sense of security that, even if these warnings
weren't meant to apply to the security of the entire transaction, a layman
might very well perceive it that way. In English: the padlock doesn't
necessarily mean you're safe. I want you to consider the amount of moving
parts and things that can be bugged or accessed illicitly in one simple
transaction, say, sending a password.

- The user's computer can have a keylogger on it or be otherwise bugged.
Password's leaked.
- The site can use both HTTP and HTTPS materials, thus letting someone listen
in on what's being sent. Leaked.
- Good ol' human error or not giving a shit. If you give your password to
someone, and they're careless, the password can get out through them.
- A security breach can happen at the remote site. Someone forgot to update
their database software and someone made off with everyone's passwords and
credit card information. Again, human error leads to a data leak.
- Hell, who says phishing can't happen over HTTPS?

I can imagine some "I'm so cool because I can write node.js" web developer
looking at this and calling it whataboutism, but that's my point. We've spent
countless manhours trying to get everyone to up security in this one specific
way, handing out Let's Encrypt certificates and getting browsers to spook
people, with the eventual goal being to outright mandate it (fuck freedom of
choice, right?), when the underlying premise of security was *bullshit* in
the first place. This is like squabbling over the difference between emptying
a fishtank using a hammer or a bullet. That box doesn't hold water anymore
either way.

This only came about because we started abusing the web for things it was
never meant to do anyway. The web started as a little research project meant
to provide global access to documents, remember? Security wasn't a concern
because it was never meant to do secure things. It was meant to let people
read papers online, essentially, and no surprises there, this is what it's
still best at.

> The project is based on the philosophy that much academic information
> should be freely available to anyone. It aims to allow information sharing
> within internationally dispersed teams, and the dissemination of
> information by support groups. Originally aimed at the High Energy Physics
> community, it has spread to other areas and attracted much interest in user
> support, resource discovery and collaborative work areas.

Yet, because people continually try to shoehorn shit into the original scope
of the project, here we are. Most of the time, whatever we're trying to do to
the internet this week doesn't even work especially well. Things continue to
bloat, pages get slower, and the works become even more of a minified black
box that your average web user can't even begin to understand, but as the
negative consequences from sending sensitive data through the magical pixie
box stack up, we can at least take solace in the fact that at least it didn't
happen over HTTP.

That doesn't mean there's no benefit to at least trying to secure things, I
suppose, I just wish we stopped throwing technology at fundamentally human
problems. If you're concerned about security, why are you still connected to
the internet at all?

I read through a lot of these smarmy "yes, you need HTTPS sweetie uwu"
articles and sites tonight, people so arrogantly pushing for something that
doesn't really change the insecure nature of the thing they're using in the
first place. (Seriously, these sites amount to "Fuck your ad-based
livelihood, fuck your freedom of choice to have legacy support, fuck your
concerns about who's actually saying what's secure, fuck you *especially, I'm
right* and you should do what I say.")

Do we have much of a choice? Do we just give up all this luxury, convenience,
and commerce for buying things locally with cash and having perfect
anonymity? No, but if you're willing to take the risk, don't expect a cute
padlock icon to protect you.