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

Doghouse
Zork v1.0
===
Enemies:
Bad Man
***
“Definitely not goodman.” //description
***
isHostile //or isNotHostile
150 // health
15//Str
10 //Def
2 // points
Inventory: Rope,Candle
***
“This is how we talk down south.”
“I can say more than one thing.”
"Have you ever been Weast"
***
---
===
Items:
CrumpledPieceOfPaper
1 //weight
5 //str
5 //def
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
    
This engine also features locked doors, combat, and enemy NPC's.  

![zorkclassdiagram.png]({{site.baseurl}}/img/zorkclassdiagram.png)

