---
layout: post
date: '2017-04-27 22:35 -0400'
author: Alec
published: true
categories: UMW
---
![jumpDaviesJump.png]({{site.baseurl}}/img/jumpDaviesJump.png)
## A game created for GBA hardware, runnable on GBA emulators.  

## Up, up, and up you'll go, where will you stop - Dr. Finlayson - no!!! 

***Davies Jump*** is a endless jumper designed for the GBA.  It stars the infamous Professor Davies as he ascends into space all while trying to avoid the clutches of Dr. Finlayson, a floating space rock.  Careful though, Dr. Finlayson is a space rock with an anger problem.  Being hit one too many times or falling out of the boundaries of the screen will lead to Davies being reset.  It isn't difficult to set up the code to run the game if you follow the instructions on the [repository](https://github.com/acarlyle/davies-jump) page.  

## The Computer Systems and Architecture Project

The project specifications were simple.  We needed to create a GBA game that included:

* A scolling, tiled background
* A minimum of 2 sprites
* 2 functions that were written in assembly code

Writing a game for the GBA is no walk in the park.  Not only is it lacking an operating system, but it has comparably low specs to the smartphones of today.  The act of writing games for the GBA is low level programming at its core.  You are required to set bits to certain values in order to access certain visual functionalities.  For example, there are 6 different graphics modes.  One of these modes allows you to have 2 tiled backgrounds, which are rotatable and scalable.  Another mode offers 3 tiled backgrounds, but only one can be rotated and scaled.  The first 3 bits of the display control register control which mode we are using.  With this in mind, the possibilites of the first 3 bits include:

		000
        001
        010
        011
        100
        101
        110
        100
        
These possibilities allow for each of the different modes to be set, and then some.  Knowing that the display control register is just a memory address that directly needs to be modified was critical to my understanding of how Computer Hardware is working together with memory.  

## Reflections

If I had to do this project again, I would want to do more with it.  I loved working on it, and I'd want to take it to the next level.  It was difficult to put together, and I feel like a full-sized GBA game would be  quite the challenge, and a satisfying one at that.
