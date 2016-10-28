---
layout: post
title: Django Rest Framework, AngularJS and UI-Router
date: 2016-10-28
category: bootcamp

---

The past two days have been a real life experience of the tortoise and the hare. The are moments when I am making a lot of progress, ticking off user story tasks and seeing visible improvements to the application. Then there are periods that a problem comes up that brings that progress to a halt. In those moments, I try to find comfort by reminding myself that I often excel when it comes to activities that are 'long and steady'. This is true in the physical challenges I take on (such as the marathon or Ironman), but also in daily behavior and productivity. I keep telling myself to 'Make progress daily'. 

(Watch the story of the [tortoise and the hare][tortise-hare] on youtube.)

That is a great philosophy, but there is also the reality that our Demo Day is November 10th. Therefore, I have to have something that has been deployed and demonstrates what I have done.  That adds a little anxiety, but I'm confident the project will be ready. 

What I accomplished the past two days: 

- completed the viewsets and serializers for my REST api (using Django Rest Framework)
- set up api service within AngularJS to consume that api data on the front end
- set up components in AngularJS 
- needed to create new views for Angular app, which meant that I had to got introduced to ui-router
- which meant... refactoring api service, controllers, components and creating states in app module to use the new routing (this was one of those tasks that took a little time)
- got templates and UI created for list of races and individual race results

What I want to accomplish today: 

- enhance the api service to provide some filtering
- create models for storing 'Grand Prix finishers'
- add 'Checkin' UI, so runners can checkin their bib numbers post race

Barriers to progress: 

- getting too obsessive about having the api do everything I would like it to right now (just need MVP for Demo Day)
- learning curve with improving the api
- getting data uploaded into the postgresql database from the csv files from race directors 

[tortise-hare]: https://www.youtube.com/watch?v=MeZe2qPLPh0

