# gopher.somnolescent.net
This is most of the setup for [our Gopher server](http://en.wikipedia.org/wiki/Gopher_(protocol)) at gopher.somnolescent.net ([proxy link](http://gopher.floodgap.com/gopher/gw?a=gopher%3A%2F%2Fgopher.somnolescent.net)). We run using our own Python 3-based server package called [Pituophis](http://github.com/dotcomboom/Pituophis), which isn't included in this repo (see below). This repo also contains the code for our homebrew Gopher search solution Gophew, which Pituophis is run through to allow searching across the entirety of our server.

## Guide to files
- **gopher directory:** Contains all Gophermaps and files being served.
- **crawler.py:** A Gopher server crawler. Dumps its results into **db.json**.
- **serverstart.py:** Gets a Gopher server running (Pituophis) and intercepts and facilitates all itemtype 7 searches (Gophew). Pituophis can be started without Gophew, though obviously without itemtype 7 handling.

## What's not included
- **SomnolCCSO:** The CCSO daemon runs separate to the Gopher server. You can get it set up for your server [by visiting its repo](http://github.com/Somnolescent/somnolccso). The database is excluded for the same reason, and also because you doing your own searches to find out what's inside is more fun than me giving you the list.
- **Pituophis library:** Omitted for redundancy reasons. You can pull the latest version of Pituophis from [its own repo](http://github.com/dotcomboom/Pituophis) or through PyPi, whatever works best for your setup.