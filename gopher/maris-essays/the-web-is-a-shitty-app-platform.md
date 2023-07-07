# The Web is a Shitty App Platform
## May 9, 2019
### From gopher.somnolescent.net, the Gopherhole of the weird lightbulb people
Bloat and inefficiency are the enemy.

---

I'm a big believer in implementing as little as possible to get the task at
hand done. I'm as minimalist as it gets. Proprietary, open source--ultimately
doesn't matter to me so long as it gets the job done as simply as it can.

So why in fuck's name did we give everything away to the Web?

Imagine this scenario: you'd like to pass a ZIP of MP3s to a friend. What are
your options? Well, not Discord, which has an 8MB upload size limit without
paying for Nitro and thus supporting terrorism. You can use Mediafire, MEGA,
or similar such sites, which throttle both your upload and download unless
you throw more money at them. Or perhaps you can use Drive, OneDrive, or
Dropbox--and support giant corporations.

Or maybe--we can use the protocol we had for this back in, oh, 1971 or so.
Called FTP.

Or, if you really need to keep it secure, you can use the separate, secure
version, called SFTP.

Really think about it for a moment: anyone can host an FTP server, using any
sized drive and OS and limited only by your normal internet speeds. There's
no file size limit, and provided you have physical access to the server, it's
dead simple and lightning fast to get files onto it. Again, if security is
paramount, SFTP is as secure as SSH and works about the same. Only hangup is
it needs a dedicated client (because overstuffing Web browsers full of
features is a *real problem*, you see), so most people would look at an FTP
link in confusion and helplessness.

So instead, giant messes of files are instead hosted on skeevy and skeevier
file hosting sites that throttle users and waste your time and, potentially,
deliver on-click ads and viruses. Their UIs are consistently terrible,
cluttered, and ugly. They're slow. They can't be crawled and archived. They
don't deserve a penny for reinventing what we'd already figured out *long
before* the days of Netscape.

With the eternal wave of normal, everyday people hopping onto the internet
since 1995 or so, we've successfully managed to train the general population
into thinking everything on the internet is either done through a web browser
or, maybe, through a video game. Websites and "programs"--usually web
browsers in their own right--have one-by-one replaced the older, quicker,
simpler-to-maintain programs using their own protocols--see FTP, IRC, NNTP,
dedicated email clients, and so on.

In their place, we've given everything up to HTTP and the web, a damn
strong resource in its own right, but made to fill gaps it was never meant
to fill in the first place. The web is good for delivering information,
static files, and facilitating interaction based on those things. Blogs are
a good example of something the web is good at. Some social media, notably
Twitter, make good use of the web's capabilities.

Instead, we've now turned it into a streaming box, a games machine, a file
transfer service, and a chat platform, all by stacking on more and more
totally unnecessary technologies like WebAssembly, which several indie dev
LARPers have assured me will revolutionize gaming as we know it by enabling
yet another one-size-fits-all solution for a variety of devices that all
work and can be interacted with entirely differently. And I guarantee you
that, even if one or two major titles adopt it, no one else will.

The web doesn't do everything. Instead of building native apps to properly
use the power of each separate device and the efficiency of different
protocols, we leave it all up to the web. We've managed to build an internet
where the same shitty service is being delivered through Chrome, not-Chrome,
embedded Chrome, and Chrome on Android, and takes advantage of none of their
strengths as a result, and in fact, comes with all the ads, shitty,
mismatched UIs, and nonsense the web's enabled in its wake.

So here we fucking are. That's why I have to struggle to send Radiohead
albums to sushi every damn time.