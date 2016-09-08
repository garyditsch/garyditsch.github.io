---
layout: post
title: Web Development Bootcamp - Day 4 - Bootstrap
date: 2016-08-26
category: bootcamp

---

The day once again started off a little shaky, as one of the challenge questions stumped me. It just means that I need to spend some extra  time on becoming a javascript and python fluent person. After the challenges we jumped into some more comfortable territory, learning and using Bootstrap to style pages.  I have used Bootstrap a few times so my comfort level was high, but it was nice to work through examples with the class and see how others use the different features and defined classes that it offers. 

### A couple new things that I learned: 

1. There is a featured called “cards” which help create elements for content. The elements are smaller boxes, but they can have other features added to them like header images, titles, etc. I have never used them in the past, but after playing around with them a little, I began thinking of several different way they would become handy.  One thing that would be an interesting challenge would be to use cards to store excepts and images from articles and then build a home page that looks and feels like a pinterest page. 

2. The other element that I spent some time on was nested columns. In theory, it makes a lot of intuitive sense, however in practice it an become fairly tricky to get some designs right. Again, with repetition comes mastery.  

### Let’s look at an example. 

Some rules to know before we start: 
- A row consists of 12 units to make up the grid. 
- It’s generally considered good practice to not add style elements to .container, .row and  (url)

What would we do if we wanted to have a row that had one column that was 3 units wide, then we wanted the remaining columns to be equal in size?  The first thought would be to have 3 total columns, like this: 

Column 1: 3 units   —— Column 2: 4.5 units — — Column 3: 4.5 units

What I found out quickly is that Bootstrap doesn’t with with half measurements. Therefore, how do I get my remaining 9 units into equal width columns?  <Strong> This is where nested rows and columns comes into play.</strong>

When you create a new row, that row gets its own 12 unit wide grid. Therefore we can nest a row inside that 9 unit wide column, then create two equal width columns by giving each column a width of 6 units (half of 12).  While it may seem like the result would be 15 unit wide row, we actually end up with our twelve unit wide row. It will look something like this: 

Row:  (3 units ,  9 units (row: 6 units, 6 units))

The key understanding here is that another way that one could interpret the “6 units” in this example is that it is 50% of the original 9 unit column. 

This is one thing that helps to have some visual reference for, so you can check out my solution to this challenge here:  [Grid Example Solution]



[Grid Example Solution]: https://github.com/garyditsch/bootcamp-challenges/blob/master/bootstrapGridChallenge.html