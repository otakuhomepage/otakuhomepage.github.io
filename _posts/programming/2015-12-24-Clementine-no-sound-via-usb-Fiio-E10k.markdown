---
layout: post
title: "Clementine no sound via usb Fiio E10k"
date:  2015-12-24 22:59:48
categories: [programming]
---
So I'm on Linux. I just got a Fiio E10k. And hooked it up. Everything seemed working. Except clementine wouldn't output audio. VLC / system sound worked fine. After some googling. The correct answer is

```sudo apt-get install gstreamer0.10-alsa```

And now I have perfect clementine audio over usb to my Sennheiser HD 650. Life is good.
