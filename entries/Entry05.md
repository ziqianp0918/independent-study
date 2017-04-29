# Entry 5: Week 5 of learning EarSketch Tutorials 
### (Unit 3 chapter 17 - 18)<br>
In week 5 I will be learning how to use code to make randomly generated music. Where I can ask for user inputs and that would change the outcome of the music.
It can be interactive instead being always the same when you listen to it. It would change and become dynamic.


``readInput()`` allows the script to prompt the user for an input. It is very similar to the ``prompt`` tag in HTML. Where it allow the website to have a pop out window asking for an input from the user.
Once we have gather the input from the user we want to use it however the input from the user comes in as a string. We would have to convert the data type before we can use the input for something else. In the documentation it gave us some data type conversion syntax such as: 
- ``str()`` which converts anything into a string. 
- ``int()`` coverts a string into a integer. 
- ``float()`` converts a string into a float. **Note** difference between an integer and a float is that integer does not have decimals while a float does. 
___

```python
t = readInput("Set a valid tempo for this song (120 - 160): ")
print "You set a tempo of " + t + "bpm"
tempo = int(t)
setTempo(tempo)
```
Here is when we ask for the user input. ``readInput("Set a valid tempo for this song (120 - 160): ")`` tells the program to have a pop out window where it would ask the user put in a valid tempo ranged from 120bpm -160bpm and the user would have a text box where he or she can put the value. 

## Booleans in EarSketch
it is the same compare to what we have learn in any other coding language.
- ``==`` means identical to<br>
- ``!=`` means not identical to<br>
- ``>`` means greater than <br>
- ``>=`` means greater than or equal
- ``<`` means less than
- ``<=`` means less than or equal
- ``and``: Takes 2 boolean inputs and returns _True_ only when **both are True**, otherwise returns False.
- ``or``: Takes 2 boolean inputs and returns _True_ when at **least 1 input is True**, otherwise returns False.
- ``not``: Takes 1 boolean input and returns the opposite (negated) boolean.
___

## Conditionals
After learning about Booleans we moved on to conditional, with ``if`` statements. 
In EarSketch you do not have to use ``end`` like we did in Ruby. We had to be careful with the indentations.
``` python
if (a > b):
    #do this if statement is true
    #if a is greater than b
    #code have to be indented 
elif (a < b):
    #do this if a is less than b
    #code have to be indented 
else:
    #do this if frist two statements is false
    #a is equal to b
    #code have to be indented 
```

___

## Data Structures
First we will be going over **List**, which is also called **arrays**. In EarSketch we use arrays to hold different elements for easier access.<br>
Here is a example:
```python
from earsketch import *
init()
setTempo(130)

#Music

#create a list of clips
myEnsemble = [RD_ROCK_POPRHYTHM_MAINDRUMS_12, RD_ROCK_POPELECTRICBASS_16, RD_ROCK_POPELECTRICLEAD_11]

fitMedia(myEnsemble[0], 1, 1, 5) # accessing index 0
fitMedia(myEnsemble[1], 2, 1, 5) # accessing index 1
fitMedia(myEnsemble[2], 3, 1, 5) # accessing index 2

#Finish
finish()
```
We created a variable called ``myEnsemble`` which contain elements ``RD_ROCK_POPRHYTHM_MAINDRUMS_12, RD_ROCK_POPELECTRICBASS_16, RD_ROCK_POPELECTRICLEAD_11`` inside a bracket ``[]``. Just like an array the elements start with the index of 0, so in this case ``RD_ROCK_POPRHYTHM_MAINDRUMS_12`` has a index of 0 and so on.
___

## Iteration in EarSketch
```python
from earsketch import *
init()
setTempo(120)

#Body
myList = ["Get", "thee", "to", "the", "console!"]

for i in range (0, len(myList)): # Stopping condition determined by list length
  print myList[i];

#Finish
finish()
```
Here we see that we have a ``myList`` array which contains ``["Get", "thee", "to", "the", "console!"]``. In order to iterate through the array, we started with a ``for`` loop where it starts with zero and it ends with how many elements there are inside the ``myList`` array. So every time the loop runs it would update the value of i from 0,1,2,3,4. And after each change, the loop would print out the value of the element in that index.
<br>
the console output is
```
Get 
thee 
to 
the 
console! 
```
You can also use arrays for the function ``makeBeat``.<br>
```python
from earsketch import *
init()
setTempo(100)

#Music
drums = [ELECTRO_DRUM_MAIN_BEAT_001, # an list of drum clips
		 ELECTRO_DRUM_MAIN_BEAT_002,
		 ELECTRO_DRUM_MAIN_BEAT_003,
		 ELECTRO_DRUM_MAIN_BEAT_004]

drumPattern = '0+0+11112+2+3+++' # each number is actually an index into the drums list

makeBeat(drums, 1, 1, drumPattern)

#Finish
finish()
```
Here the ``makeBeat`` fuction takes in all of the music listed in the array of drums. Then it starts on track 1 and measure 1. It start using the ``drumPattern`` to make the actual beat of the music.

## Takeways
1. *look closer.* don't just quickly skim through the documentation, the creator made it for a reason, to help others learn the topic faster. When given an example look closely at the code not just oh I know what this line of code does and so on. Learn how each line of code work with each other and really read the **comments** that are left by the creator. In one of the example about the code ``drumPattern = '0+0+11112+2+3+++'`` I had no idea that what the numbers within ``drumPattern`` mean because the previous lesson taught me that you can use 0,1,-,+ to make beats play in the ``makeBeat`` function. But the creator left helpful comments that say "each number is actually an index into the drums list". Without reading this comment I would have no idea what the number actually mean.
