---
layout: page
status: publish
published: true
title: Go for the bigger column. Always.
date: '2015-01-14 07:20:38 -0800'
date_gmt: '2015-01-14 07:20:38 -0800'
categories: [programming]
tags: [programming]
---
<p>I use a lot of varchar columns in mySQL. One of the things that I always run into is how much varchar to allocate? After all, you don't want to be wasting space right? So I always try to estimate it as close to the lower bound as possible?</p>
<p>I've learned now is to always try to overestimate. And then overestimate some more. I've never had a time where making I needed to shrink the size of the varchar. I've only encountered scenario's where I had to change the varchar to something bigger.</p>
<p>And it's horrible when that happens. It's painful and bad. In the case of what happened to me recently... I lost data because mySQL truncates your shit without warning. I know that postgres will at least throw an exception so that you know. Either way, you're going to be losing data.</p>
<p>It reminds me of the youtube gangnum style video where the guy used an integer for the counter thinking a video couldn't possible reach it. Regarding that... I don't know why he didn't use an unsigned integer. I digress.</p>
<p><strong>tl;dr - always go for the bigger var char. Don't preemptively optimize. Make it 3x bigger than what you think. You never know what crazy customers &#47; you will want to do in the future</strong></p>
