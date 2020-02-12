+++
author = "David Makogon"
date = 0001-01-01T00:00:00Z
description = ""
draft = true
slug = "hackeddb-all-your-database-are-belong-to-us"
title = "HackedDB: All your database are belong to us"

+++


Recently, there's been a spate of database hacks in the news. Some of these are related to your personal data being compromised, thanks to someone infiltrating a database and publishing it for the world to see. There are so many of these, that Troy Hunt found a need to establish haveibeenpwned.com, just to help people track their public data!

it's pretty bad, finding out your personal info has been siphoned off, and shared to the world. But let's consider another type of database hack: ransoms. Consider this little example, where I launched a MongoDB instance without any security enabled. It only took about 48 hours for me to discover a new Collection in my database:

![Ransom note placed in a new collection][]

I know what you're thinking:

> *How stupid of me to place an un-secured database on the Internet!*

 Nobody would do this, right??? Well... I won't comment on any assertions you might have regarding how stupid I am, but I will comment on how *common* this scenario is. Better than commenting: let me walk you through some real-life security holes, and how you can patch them up on your own databases, so that you don't get the opportunity of showing off a ransom note you received.
 
 ## Public ports
 
 Thanks to the cloud, Virtual Machines are near-trivial to spin up: Choose an OS, a size, a region, and a cup of coffee. Your VM will be ready before your last sip.
 
 A few minutes later, you've ssh'd (or RDP'd) into your new VM, installed a dataabase package, and you're up and running.

