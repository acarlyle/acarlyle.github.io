---
layout: post
date: '2017-04-27 22:42 -0400'
author: Alec
published: true
categories: UMW
excerpt: ''
meta: ''
---
![zorkSp00k.png]({{site.baseurl}}/img/zorkSp00k.png)

## A text adventure game engine that runs demakes of Zork.

One of my favorite projects I made while at Mary Wash was bork.  I love ye old text adventures of yore, and creating an engine that can generate such games was basically the coolest thing ever.  This was created way back in Object-Oriented Design, which was young in my Computer Science endeavors.  

### Design

The engine was written entirely in Java.  Not only did the assignment introduce Object-Oriented concepts, but it was the first project where we had to work with other people using git and linux.  It can read in any .txt file formatted as so:

	Zork v1 save data
	Dungeon file: /home/acarlyle/borkProject/src/edu/umw/acarlyle/bork/doghouse.bork
	Room states:
	Cell
	beenHere=true
	Enemies: Bad Man
	---
	Flooded Stair
	beenHere=false
	Contents: CrustyKey
	---
	===
	Adventurer:
	Current room: Cell
	Inventory: Candle,CrumpledPieceOfPaper
	Health: 5
	Str: 12
	Def: 10
	Score: 20

![zorkclassdiagram.png]({{site.baseurl}}/img/zorkclassdiagram.png)

