---
layout: post
title: Week Two - Python and Object Oriented Programming
date: 2016-09-07
category: bootcamp

---

The past week was focused on learning python. We have used python in all of our morning challenges. Python was a part of the pre-work we had to complete, before starting the bootcamp, but we are now digging into it. Having used python for some data analysis, I believed I had a better understanding then I did. That being said, I feel that I am learning the concepts more each day. The repetition is a necessary part of my learning process. I also enjoy using the language, because it is a very friendly language to read and write. 

The one thing we spent a lot of the week focused on was object oriented programming. This was completely new to me, other than being introduced to the idea when I launched the Central Kentucky Grand Prix site using Django. However, I followed a tutorial to get that site up. I clearly did not fully understand everything that was happening. 

One of the concepts, that I feel I am finally picking up is the value and use of classes.  Classes are a set of data and functions that are used with that data. Mentally it helps me to think of them as a structure or framework for data to be stored. The class doesn’t actually store the data itself, but is used to create an instance of the class. 

Let me use an example to see if it helps clarify it, for you and for myself.  Last weekend was the start of college football, so in the spirit and excitement of the season, let’s make a college football team class (Cfb_team).

Some attributes that a college football team may have include:   name, coach, conference, mascot, and number of national championships. To create this class would look like the following. 

```python
class Cfb_team():
    """Has attributes of conference, coach, mascot, national_titles"""
    name = ""
    conference = ""
    coach = ""
    mascot = ""
    national_titles = 0

    def __init__ (self, name, conference, coach, mascot, national_titles):
        """ helps set up instance of the class """
        self.name = name
        self.conference = conference
        self.coach = coach
        self.mascot = mascot
        self.national_titles = national_titles

```

As mentioned, the class is just a template for the data we want to store and access. At this point, what needs to happen to get information stored for the greatest college football team of all-time, the Huskers? In this case, we need to create a copy of the Cfb_team class, with the Husker information. The actual term used for this is to create an ‘instance’ of the Cfb_team class. A function that could be written to help create a team object might look like this: 

```python
def create_team(name, conference, coach, mascot, national_titles):
    """ this function takes the arguments and them passes them into the class creating the team instance """
    team = Cfb_team(name, conference, coach, mascot, national_titles)
    return team
```
Then actually calling that function, passing the Husker arguments would look like this: 

```python
huskers = create_team('Huskers', 'Big 10', 'Mike Riley', 'Herbie', 5)
```
When you have that object, you can then do all kinds of things with it. Below, I simply print out the attributes to the console. 

![alt text][husker_class]

[husker_class]: /assets/img/husker_class.png "Husker Class"






