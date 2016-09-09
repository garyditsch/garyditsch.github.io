---
layout: post
title: Circular imports and python
date: 2016-09-09
category: bootcamp

---
I started ["refactoring"][refactoring] my text adventure game, Six Days to Game Day, which I knew would be a challenge. The first step that I wanted to accomplish was to pull all my code into different files. I initially wrote the game in a single file, then as I made progress, continued to simply add features to that file. The major issue that I see with this practice is that it creates a very long file and becomes challenging to review. The benefits that I thought would happen from refactoring: 

1. The code would become more readable
2. I could pull code together that served a similar purpose
3. I would learn more about python imports and modules

To start, I simply pulled each class into its own file. There were a couple functions that didn’t belong to a specific class, but worked with one of the classes I had defined. Secondly, I added all the required imports to the top of each file. I had a moment of optimism that everything would work after this - but it didn’t. I spent an hour trying to make some minor edits to the importing statements. I was thinking I had improperly imported one of the modules. When that continued to be unsuccessful, I decided to take a break. 

I went for a six mile run. Running is not only great for my health and mood, it is also a time that I often have moments of insight and inspiration. That did not happen for this issue. Despite not having any moment of insight, I did come back to the problem with renewed motivation. 

The next step I did was take some time to learn about the main issue I was having, circular importing issues. This question and response on StackOverflow was really the most helpful information that I read: [“Circular Imports in Python”][circular-imports]

This new information allowed me to realize that I needed to take a step back and rethink the structure of my game. I ended up with this structure: 

- Main.py : has the basic game structure
- Game.py : has game setup function, has main game play loop, keeps track of what day of week the player is on
- Player.py : creates the player, gets user input about their player
- Weekday : keeps the functions for all the training actions, along with the actions on game day
- Display : has content for the menus to display to the player

I am much further along in having a working game again, with cleaner and more organized code. While I was a little bummed about having to rewrite so much of the code, it has been a good learning process. It was also not nearly as difficult writing the game this time, because I knew how to approach many of the challenges I had faced the first time around. There were components from the original game that I could simply copy and paste into the new version, so that was also beneficial. 

At least now I understand what a circular import is in python and that it is not allowed.  


[refactoring]: https://en.wikipedia.org/wiki/Code_refactoring
[circular-imports]: http://stackoverflow.com/questions/9252543/importerror-cannot-import-name-x






