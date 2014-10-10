---
layout: post
title: Beginning Again (this time in earnest)
---

I've decided to make yet another attempt to get back into development, at least, I intend to (confidence inspiring, no?). My hope is that by putting my thoughts down in a public place, I'll at least keep myself more honest.

I'm not new to it, but it sure feels that way. It's been 6 years now since my last full time job as a developer. I've kept a toe in it since leaving, but it hasn't been enough.

##Why?##

 Creative outlet. Personal fulfillment. Pursuit of something more, something satisfying. Can these be achieved? Creative outlet, sure, but the others are more waypoints off in the distance.

 ##Why Now?##

 2 kids, full-time job, weekends taken up with housework, birthday parties, extended family visits. This is something that fits into my schedule right now, productive work I can do after the kids go to bed.

 ##Where am I coming from?##

 I definitely can't say I've consistently focused on any one thing profesionally. I started in IT out of college, doing general support for a few years before jumping into full time Ruby on Rails position at a startup. This was during the social networking craze - everything was trying to be social, figure out how it fit in - so that's what I did, built a series of "me too" social networks. More than anything, I learned that diving in headfirst is the only way to learn.

 I had the fortune of going RailsConf and FoWA in 2008, which exposed me to some cool technology, and introduced me to some very talented and intelligent people. I also worked with some incredibly smart people at the startup too. This is where I developed my relationship with code and respect for the people who are crazy good at it.

 By the end of 2008, I could see that the startup wasn't going to last; I was recently married, a new homeowner, and I was looking for something with more promise. so I left and returned to IT.

I've been working in IT ever since. I've developed a few applications professionally since - a touch-enabled keypad in Ruby on Rails (TDD and my first gem), a system status page (Zend framework), several Wordpress sites for various projects and dabbled in Node.js with all of them - but I'm not a full time developer. I'm barely even a part time developer.

##Where do I want to go?##

C# and .NET. It can power websites, desktop apps, APIs, and now every mobile platform via [Xamarin](http://xamarin.com/). It's one language that can do it all. It's a strongly typed language, meaning I can't just create a variable and assume the interpreter will know what kind of type it is (which is found in Ruby, PHP, and others). C# types are cast when variables are defined or objects are assigned to a variable.

C# is a compiled language, another new-to-me concept. C# compiles into an intermediate language, which is then translated into platform specific machine code at runtime as it is needed, or "Just in Time". The nice thing about this C# can leverage libraries written in other languages that also compile into that intermediate language, or that leverage the .NET framework.

C# leverages Visual Studio, which, though daunting at first, contains so many nice features beyond code completion (which Microsoft calls Intellisense). Installing Visual Studio, as "bloated" as it may seem at 14GB (but hey, storage is cheap) is easier than setting up a local development environment for PHP, and in most cases Rails if you're like me and don't use the built-in rails server. I don't have to worry about an update to my OS breaking Apache, MySQL, or any of the dependencies I painstakingly compiled with a multitude of flags and options.

Then there's Azure websites - a platform that integrates with Visual Studio that includes scaling, load balancing (across multiple physical locations), metrics and more all bundled up in a nice *and cheap* package. Seriously? You mean I don't have to standup my own servers (I know, I know Chef is a thing), configure a lengthy deployment script, manage my reverse proxy and application runners? Sign me up!

Oh, and parts ASP.NET are going open source with the [vNext release](http://www.asp.net/vnext "ASP.NET vNext"). That's some street cred with the cool kids out there.

My hope is that all of these features will make my life easier as a developer, and make me spend less time digging out. 

Ok, enough fooling with my first real blog post - I'm publishing this thing.