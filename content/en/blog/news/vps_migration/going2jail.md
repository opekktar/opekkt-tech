---
title: "Going to jail"
date: 2022-03-08T23:26:06.000Z
draft: false
description: "Going to jail"
tags: [VPS, Vultr, Hosting, SSH, Jails, Documents, NextCloud]
catagory: Documents
---
Matching blog post to [Going to jail](/docs/server/vps_migration/going2jail) @ [Opekkt.Tech/Docs/](/docs/)

# Getting thrown in jail

This was a fairly stressful venture as I did it while at my day job working as a medical receptionist (I've been unsuccessful so far, getting back into IT after being laid off). So this was done while answering phones, booking appointments, and checking clients out. Needless to say the stress level was a bit high for making a mistake there or here. But I'm addicted to IT and technology so I have to play 24/7/365 or I will probably just die of boredom.

I will create docs and post on how I setup the database jail and NextCloud© jail in future installments. My goal here was to just get things moved off a host instance and into jails and consolidate things a bit as I use Cox Communications at home for internet and they are notoriously slow on upload speeds, so that really slowed down my NextCloud service. _The server at home is awesome having 72GB of ram and 8TB of mirrored ZFS disk. But all the power in the world does you no good if your internet provider throttles your upload to less than 6 Mbs. (That's not a typo) Here is a word of advice; never run an OONI probe[^1] on your internet provider in case they hold grudges. All stories for another day._ And with an ~~80G~~ 128G NVMe, I think I'm good for a while as I mostly just use CalDAV and WebDAV services.  My photos still reside on Google© for now. That will be another project to document in the future.

So far I pretty happy with Vultr©, my configuration thus far and the performance; yes I need to compress some images and convert to .webp and there are some tweaks I could make elsewhere I'm sure. But things are looking good so far.

I know everything below is in the docs section as well: But how else can I convey my excitement when I finished the migration and ..........................

> At this point I say "Hold onto your butts" and reboot the VPS instance.

> Within about a second I browse to <a href="/" target="_blank">opekkt.tech</a>, <a href="https://opekktar.online/" target="_blank">opekktar.online</a> and <a href="https://nc.opekkt.tech/" target="_blank">nc.opekkt.tech</a> and all 3 sites were up and operational. I then ssh into the host ```ssh -p 5000 titania``` and then ssh into the jail ```ssh caddy``` and this all worked as well.

> Then I jumped out of my char and screamed "Holy fucking Shit!!!" Yeah, I was surprised it worked.  There were a lot of moving pieces and not shutting down before taring up a jail, hell using tar instead of bastille export for that matter. So many configs to make typos on. Yes I'm a happy camper :)

[^1]: Born in 2012, the <a href="https://ooni.org/about/" target="_blank">Open Observatory of Network Interference (OONI)</a> is a non-profit free software project that aims to empower decentralized efforts in documenting internet censorship around the world.
