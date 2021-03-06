---
layout: post
title: "D6.5 Experiments (Part 2)"
---

I've been trying to do an install of Documentum using the Linux/Oracle downloads without much success. This may well be more on the Oracle side of the fence, but this started when I put Oracle XE(10.2.0.1-1) on a newly installed CentOS 5.3 virtual machine, and then tried to get Documentum (6.5SP1) installed and configured, only to get the majority of the way through and be told that the minimum is Oracle 10.2.0.3,  <strong>despite what the release notes say</strong>.
<!--more-->
Since 10.2.0.1-1 is the latest Oracle XE, I concluded that it must not be supported and moved on to trying 11.1 (Standard One). The biggest downside to this is that this Oracle installer is far less friendly than the XE installer, and at the end of it, I am not left with a TNSNAMES.ORA which Documentum needs. I am not an Oracle expert by any means, I would prefer to use PostgreSQL or MySQL, but they're not a supported configuration. Even ignoring 'supportability', since this project is only experimental anyway, there is no information on whether it is even possible to get it running using these databases. Since there is a large amount of mapping/optimization between DQL and the underlying SQL I would tend towards it not being possible.

Does anyone have any advice or instructions for getting D6.5SP1 installed from scratch on linux? Failing that I will persist with my attempts, and let you know how it turns out.
