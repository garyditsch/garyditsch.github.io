---
layout: post
title: Bootcamp - Learning Jekyll
date: 2016-08-25
category: bootcamp

---

Yesterday we spent the day learning Jekyll and then implementing it into our portfolio sites. Jekyll is a static site generator that makes it very nice to create simple blogs and websites. Another nice feature is that it can run on GitHub pages, which provides hosting.

In the past decade (or longer), I’ve done many different things to host websites and blogs. I have created sites from scratch, self hosted WordPress sites, used WordPress.com and recently I have been using full service site builders. A few examples of sites that I have created and currently manages are:

– Endurance Base Camp (self hosted WordPress)
– my.endurancebasecamp (hosted WordPress platform)
– Active Lexington (Squarespace)
– Central Kentucky Grand Prix (Django / python)
– garyditsch.com (WordPress.com)

As you can see, I’ve used and tried many solutions. The purpose of the site dictates what makes sense as the solution. In order to learn from this project and jump into Jekyll with my portfolio for the bootcamp, I decided to try and port my garyditsch.com content from WordPress.com to Jekyll. Here are a few things I learned:

##Benefits of Jekyll:

*It can be hosted on GitHub for free

*It integrates with git very well (kind of understood since it’s on GitHub), so my blog and pages will have versioning

* It uses markdown, which is handy because I dislike the WordPress editor (I actually write in Scrivener and then copy / paste into WordPress)

*I like the idea of each page being statically built

##Moving Content from WordPress to Jekyll:

*I was a little intimidated to get started on this because I thought the process would be very difficult, it wasn’t.

*There is a Ruby gem that you can install that helps with importing the content.

*WordPress exports your posts into a handy xml download.

*Once you have your exported posts, you run the install … and … oops, there is an error message that instructs you on the other dependencies that need to be installed.

*Run the import script again and it all magically appears.

##Issues I had while doing the import:

*My initial import seemed to be broken and I couldn’t figure out why, so I deleted everything

*I went back to my WordPress site and exported the most recent posts so that I only had a little bit of content to work with

*Once I imported those posts, I realized that it was all importing fine, it was my template that was breaking the display, so once I fixed the template – Jekyll rebuilt the pages and everything worked as it should.

*Another issue that I may try to fix is that the import brings the posts over in HTML, while Jekyll prefers markdown. The HTML works ok, so it probably isn’t something I fix for every post, however I may find a way to more programmatically change a post to markdown prior to importing.

I now have my most recent posts on my portfolio site, however I have some design changes that I see want to make before sharing it with the world. That puts me in a very strange place today. I committed to post daily about my bootcamp experience, so I will put up this post. However, I’m going to be posting about moving from from WordPress to Jekyll on my WordPress.com site. That feels very inappropriate. This post will live on the portfolio site soon enough.