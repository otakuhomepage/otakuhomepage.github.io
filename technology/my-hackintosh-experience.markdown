---
layout: page
status: publish
published: true
title: My Hackintosh Experience
date: '2014-06-02 08:07:57 -0700'
date_gmt: '2014-06-02 08:07:57 -0700'
categories: [technology]
tags: [technology]
---
<p>I previously had no experience with installing OSX on windows and stuff. I did quite a bit of intensive research but I never got around to doing it fully because I didn't feel like doing it on top of learning iOS development.</p>
<p>Since I've already learned iOS development and I actually now want to create apps in my spare time, I finally decided to take action and make my hackintosh.</p>
<p>I originally wanted to use Mountain Lion since it's older and more stable so I researched how to install Mountain Lion with iAtkos. This is the <a href="http:&#47;&#47;www.instructables.com&#47;id&#47;How-to-install-OS-X-Mountain-Lion-on-your-PC-with-&#47;?ALLSTEPS">link<&#47;a> that I used originally.</p>
<p>The installer booted and everything installed, but then it hung on the first boot. Blargh. Bullshit I'm thinking.</p>
<p>Alright then, let's just try Mavericks. I search for Mavericks and find that Niresh Maverick distro with a guide <a href="http:&#47;&#47;www.macbreaker.com&#47;2014&#47;01&#47;install-osx-mavericks-on-pc-with-niresh.html">linked here. <&#47;a>So the thing about Niresh is that it bundles a lot of the post installation process. The drivers and the post installation process is suppose to be mostly automated. Cool!</p>
<p>I try and go to his site and download his shit. Fucking retarded. There's a mandatory share process or wait for 10 minutes thing. I probably could've hacked the javascript with firebug, but I had a bricked laptop and no firebug on my windows machine. So I just waited it out. Every single link on his damn site has a countdown timer or share this shit. It pisses me off so much. I just waited, but I was annoyed.</p>
<p>Fast forward to post downloading his shit after rage. Made the USB and it boots. As I'm installing, I realize my touchpad is not working. Uh oh, not a good sign. I plug in a mouse to proceed with the install and cross my fingers. Bam! It works. Sweet! After the boot I realize that wifi and my touchpad is not working.</p>
<p>Google google google, decide to try out multi-beast to install some kext files. Use MultiBeast to install some random drivers in an attempt to fix my wifi. Fuck. I just bricked my previously working install. I tried to manually fix it by removing the installed kexts, but it didn't work out. Fuck it. Just reinstall from the USB.</p>
<p>Reinstall from the USB completes, it's now 6am Sunday so I decide to sleep. Wake up at 3pm and then have food and continue. Search search search, nothing comes up. I kept thinking my wireless driver was a realtek... and it turns out it's an atheros! Blargh. I need to check shit and be more thorough.</p>
<p>Google for the kext for my Atheros which happens to be AR9285 and end up at this <a href="http:&#47;&#47;www.osx86.net&#47;files&#47;file&#47;703-atheros-ar9285-ar5b95&#47;">link. <&#47;a>Thank goodness for the helpful commenter. I go and edit the file. I tried to do sudo open Info.plist file, and I can't edit it. Well then, time to do sudo vi! It works, and I insert the new line corresponding to device id "pci168c,2b" and save. Reboot, and cross my fingers.</p>
<p>After reboot, no hang! Woot! Aaaaand.... my wifi is working! Bahahahhaha. Now, only outstanding part is my touchpad. With my wifi working, I set up Synergy. Which is a really cool KVM software I'll write about some point in the future.</p>
<p>So far, I've invested probably my entire weekend to get the Hackintosh up. I'm still missing the touchpad, so it's still a work in progress. But I'm pretty happy thus far. I just hope in the process of installing the touchpad, I don't brick it. I feel like such a badass simply knowing how to use sudo and vi. :)</p>
<p>I think I make like $20 an hour, so...&nbsp; I've spent ~$500 this weekend to build a 16gb sandy bridge macbook pro. Teehee. I'm pretty happy. My laptop has an SSD and 16gb of ram. Supposing it takes me double the time to get it working, I still save over $1000.</p>
<p>Screenshots and pictures will be coming once I get touchpad working.</p>
<p><strong>Edit: TRACKPAD WORKING!!! <a href="https:&#47;&#47;github.com&#47;RehabMan&#47;OS-X-Voodoo-PS2-Controller&#47;wiki&#47;How-to-Install" target="_blank">Link Here<&#47;a><&#47;strong></p>
<p><strong>tl;dr - almost have my hackintosh working! woot woot!<&#47;strong></p>
