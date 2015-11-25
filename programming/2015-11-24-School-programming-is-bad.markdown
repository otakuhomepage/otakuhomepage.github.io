---
layout: post
title: "School programming is bad"
date:  2015-11-24 02:49:32
categories: [programming]
---
I just had this thought on why school programming is bad. Think of this as a /r/showerthoughts. But basically... I remember in school I was taught proper OO programming and inheritance. And they asked you to write this program in a specific way following OO principles and of course (using inheritance).

The thing that this makes me think is that... school is so far off from the real world. First of all... the reality is that in programming there is pretty much never one true way of doing things. If you give a task to two different engineers... you'll most likely end up with two different implementations unless the problem was trivial. University teaches the correct and incorrect way... and that's not reality. It really annoyed me because I lost 70% of my grade by ***not*** using inheritance. Blargh. 

The other thing is that... inheritance fucking sucks. This is my personal opinion obviously. But after talking with a bunch of other engineers and seeing inheritance used in code bases... it almost always ends up in a horrible situation. The reason is that... inheritance always looks like a good idea initially. But then... you keep inheriting and at some point in time the behaviours become crazy complex and when you change a base class you impact like everything. To make a change you have to end up subclassing the parent class and then making your tiny specific change. It's just... horrible. I think that's why go is so amazing. No inheritance. Good riddance. 

***tl;dr - academic programming and learning from university is way different fromt the real world***
