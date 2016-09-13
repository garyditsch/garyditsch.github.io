---
layout: post
title: Creating virtualenv with correct python version
date: 2016-09-13
category: bootcamp

---

I have a very quick lesson to share today, but one that I suspect creates issues for many individuals as they begin using virtualenv and virtualenv wrapper. Prior to the quick tip, I want to share a few of the reasons someone would use a virtual environment.

When you are working on a project, you will often find other packages that you want to import. As time progresses, some of those packages will be updated, which means you will have a decision to make:  

* Do you import the most recent version, which may require you to update other parts of your project that are no longer compatible?
* Do you use the older version, which you know currently works within your project?

By creating a virtual environment, you can use the second option, keeping all of your package versions constant within the environment. One example that I have, is that I have a virtual environment for a web project I work on, but then a separate environment for data analysis work. The required packages for either type of work is dramatically different, which makes the use of virtual environments not only useful, but necessary. 

A second suggestion, when using virtual environments, is using using virtualenv wrapper. I had not been using virtualenv wrapper, but it was something we set up as part of the bootcamp. I wish I had just started using it from the beginning, as it makes managing the environments much easier. The simplicity of using the “workon” command to change into an environment, is so much better than my previous behavior of:  cd into folder, then activate the environment. It’s also handy to be able to list all your environments, as the number increases with the number of projects you have active. 

The main tip today:  Be certain to create the virtual environment with the version of python that you need. 

Twice yesterday I created a virtual environment with the default python version (which is 2.7.11), when I wanted to use python 3. 

Here are a couple stack overflow posts that helped me get past this issue: 

- [How to list all your virtual environments] [list-env] 
- [How to create a virtual environment using python 3] [python3-env]



[list-env]: http://stackoverflow.com/questions/7212140/list-all-virtualenv
[python3-env]: http://stackoverflow.com/questions/23842713/using-python-3-in-virtualenv






