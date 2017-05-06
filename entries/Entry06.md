# Entry 6: Last week of learning EarSketch
Unit 3 chapter 19 - Finished

``newList = oldList[startIndex: endIndex]`` This is how can you cut clips into a new clip. The startIndex is inclusive while the endIndex is exclusive. This is super useful let's say that you wanted a section of the music clip, however it is in the middle of that clip. What you can do is to make a new variable that cuts the original clip into the sections that you want. Now when you make your music you can simply refer it back to the variable and not need to keep cutting the piece of the music you like and would like to use.
<br><br>
``newList = listA + listB`` you can also use the (+) to combine different variables. As an example this can be used when you want to combine two different beat string together to make a longer beat string that you want to use it later.  

``randint()`` is a function from Python’s random API, that mean we have to import it in the setup of the script. Just like we import the EarSketch API with ``from earsketch import *``, the random API is imported with ``from random import *``. Once we have ``from random import *`` then we can start using the function ``randint()``. 

- ``randint(min,max)``: take in two arguments, a minimum and maximum, where both numbers are inclusive. Unlike other functions, we have learned so far where usually the first argument is inclusive while the second argument is exclusive. The reason we use this is because the EarSketch library does not contain any random function where we can use to make random music. We can not have a function that would pick a music clip from an array of music clip and use it. That way we can create a program that gives random music every time it runs. Making it fully dynamic and interactive.
___

# Tinker short music clip

```python
from earsketch import *
from random import *
init()
setTempo(120)
#track 1
fitMedia(HOUSE_ROADS_PIANO_002,1,1,3)
fitMedia(HOUSE_ACOUSTIC_PIANO_003,1,3,4)
fitMedia(HOUSE_ROADS_PIANO_007,1,4,6)
# track 2
fitMedia(RD_RNB_PIANO_3,2,1,3)
fitMedia(RD_RNB_PIANO_2,2,3,4)
# track 3
fitMedia(Y05_PIANO_2,3,6,8)

#effects on track 1
setEffect(1,VOLUME,GAIN,12,4,-40,6)#volume drop at the begin
#effects on track 2 
setEffect(2,VOLUME,GAIN,1,3,10,4)#a very small increase of volume for track 2 
#effects on track 3
setEffect(3,VOLUME,GAIN,-60,6,10,7.5)#rise in volume followed by a drop in volume
setEffect(3,VOLUME,GAIN,12,7.5,-30,8)
finish()
```
[listen to the music HERE](https://clyp.it/zhmtdcdu#)

Making music is not hard, however, I notice that making good music is hard. As I listen to more and more of EarSketch's existing music clips I found them to be limiting. Due to the fact that most of the music is pre-determined and I would need to keep listening to many of the clips before I found something I think is usable. If I want to use a part of the music then I would need to write code which I would need to get the music clip first then find out which measure is where the beat I wanted. Then I would need to cut that portion of the clip out and set it as a new variable. Only then can I use that single beat or part that I liked. I predict that it is going to be a very time-consuming process if I want to take a song and try to make it within EarSketch. I would need to find each individual note to make a certain string of sound come together. 
___

# Takeways
1. **What you are given might not always be the best. So find what you need or make it yourself.** Since I notice that using the pre-determined music clip is going to be inefficient. I would either need to find alternatives to find the beats I want or I am thinking of simply making the beats myself, record it and upload it into EarSketch. It might not even be the best idea but that what I have at the moment.
2. **Trial and Error.** Making music in EarSketch is all about trial and error. Find a clip of music you like? Well, time to put it into your code and see if it sounds good with what you already have. If it does not, then listen to more clips and find the next clip that might go well. 