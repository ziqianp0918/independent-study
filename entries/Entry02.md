# Entry 2: Deciding on EarSketch
I have finally decided to use my independent study time for EarSketch. After spending all weekend diving deep into Gosu I find out that I do not really like
how the program works. The way I have to set it up and how I can't really work on it in school and then transfer it back at home. Since I use a window at home and the school's computers are Macs, I have to change how I run the program every time I take it back home. The process becomes very annoying to do 
every time I take the project I worked on in class back at home.
___
## EarSketch Tutorials
Frist step I did to start learning EarSketch is to start with the lessons EarSketch had built in on the side of their program. So far I have got to chapter 1 unit 5 lesson 1. They start with the basic syntax to just get one sound running.
<img src="../images/ear.png" style="width: 300px;" /> <br>
There are many things you need before you can start your project. Here is a list of them you *Must* have before starting.
* ``from earsketch import *``
* ``init()``
* ``setTempo(number here to set how fast music goes)`` Number can range from 45-220.
* ``finish()``
Make sure you have these 4 things before you start putting music in.
___
Any music input must have ``fitMedia(clipName, trackNumber, startMeasure, endMeasure)``
___
## Adding effects to a clip of music
Syntax is: ``setEffect(trackNumber, effectName, effectParameter, effectValue)``
Within the effects, there is a term called "Envelopes". These are the same as adding effects to a clip of music however, it is for *part* of the music not the whole entire
clip.
___
## Takeaways
1. if possible try out the documentation that is written by the creator of the app because usually they go more in-depth on how to use their program.
2. When you come across a part of the code you do not understand try to change the value and see what happens. For instance, I did not understand the ``effectvalue`` part of setEffect 
what I did was change the values to each extreme end of the Spectrum and listen to what effect it had on the music.