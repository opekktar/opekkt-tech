---
title: "Setup GitLab Repo"
date: 2022-03-03T12:35:11.000Z
draft: false
description: "Setup GitLab Repo"
tags: [git, GitHub, GitLab, NAS, Backup, rsync]
catagory: Documents
---

Matching blog post for [Setup GitLab Repo](/docs/server/setuprepo) @ [Opekkt.Tech/Docs/](/docs/)

I suppose having worked in the disaster recovery industry, I have developed the mind set that, hardware always fails, services always fail, power always fails, service providers always go down. Now eliminating all variables is impossible, unless the money, time, and knowledge is vast and endless. For me being unemployed, having what money I do make being garnished and not even having enough for the basics that most in this country enjoy. I am very limited on my options. I use rsync to a local NAS server in my apartment, then I mirror to another server with external drives I can unplug and take off site and I have two workstations that are identical kept that way via rsync as well. Of course for development work my primary repo is GitLab (Private) and then I mirror to GitHub (public) depending on files. Of course depending on where I start my project from this is sometimes reversed :)
