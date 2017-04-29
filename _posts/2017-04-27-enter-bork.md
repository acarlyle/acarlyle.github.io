---
layout: post
date: '2017-04-27 22:42 -0400'
author: Alec
published: true
categories: UMW
---
![zorkSp00k.png]({{site.baseurl}}/img/zorkSp00k.png)

## A text adventure game engine that runs demakes of Zork.

One of my favorite projects I made while at Mary Wash was bork.  I love old text adventure games of yore, and creating an engine that can generate such games made for literally the best project ever devised.  This was created way back in Object-Oriented Design, which I was young in my UMW Computer Science endeavors.  The game engine was written entirely in Java.  Not only did the assignment introduce Object-Oriented concepts, but it was the first project where we had to work with other people using git and linux.  We also learned how to create UML diagrams to plan out our project:  

![zorkclassdiagram.png]({{site.baseurl}}/img/zorkclassdiagram.png)

The diagram itself is a little on the cluttered side, but it clearly represents the design of the game engine.  You can see several different commands available to the user, and those are created with a CommandFactory instance.  It can read in any .txt file formatted as so:

	Doghouse
	Zork v1.0
	===
	Enemies:
	Bad Man
	***
	“Definitely not goodman.”
	***
	isHostile 
	150
	15
	10 
	2 
	Inventory: Rope,Candle
	***
	“This is how we talk down south.”
	“I can say more than one thing.”
	”Have you ever been Weast.”
	***
	---
	===
	Items:
	CrumpledPieceOfPaper
	1 
	5 
	5 
	read[AddScore(3),Wound(-1)]:WELCOME TO THE DOGHOUSE (BARKING).
	examine:It appears to be....a piece of paper..?  With writing on it..?
	---
	Candle
	3
	0
	0
	wave[Unlock(Moon Hall)]:You make spooky
	---
	===
	Rooms:
	Cell
	Contents: Candle
	Enemies: Bad Man
	You are in a small, windowless room.  There is an empty mattress resting on the floor. A
	flickering candle is illuminating the cell door, which is hanging ajar.
	---
	===
	Exits:
	Cell
	n
	Moon Hall
	---
	===
    
    
Special features of this engine include locked doors, combat, and enemy NPC's.  Instructions for running the engine with custom/provided dungeons can be found on the project's [repository page](https://github.com/acarlyle/bork).  

## Reflection

If I had to make this project again, I would of course add more features to the engine.  There's limitless possibilites here, but I'd really want to include rooms that can rotate and enemies that can roam the dungeon of their own accord.
