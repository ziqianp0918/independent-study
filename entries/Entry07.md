# Entry 7: Using random

This is week 7 of my learning in EarSketch, it is closing in to the date of my final project. Just before I make my final project I want to refresh my mind about all of the concepts I have learned in during the course. Here is me practicing the ``randint`` function.

```python
from earsketch import *
from random import *
init()
setTempo(110)
#music list 
music = [RD_EDM_ANALOGPLUCK_1,RD_EDM_CHORDPART_2,RD_EDM_ELECTRICLEAD_1,YG_EDM_SNARE_BUILDUP_1,RD_EDM_ANALOGLEAD_3]
bass = [HIPHOP_BASSSUB_001,HIPHOP_SYNTHBASS_004,HIPHOP_SYNTHBASS_005,RD_EDM_WARMBASSLINE_1,HIPHOP_DUSTYBASSLINE_001]
breaks = [HOUSE_BREAK_FILL_002,HOUSE_BREAK_FILL_003,HOUSE_BREAKBEAT_026,RD_ELECTRO_DRUMROLLBREAK_3,HOUSE_BREAKBEAT_003]

#from measure 1-9 loop and do the following
for i in range(1, 9):
  index = randint(0, 4) # Generate a random index number between 0 and 4
  fitMedia(music[index], 1, i, i+1) # Use the random index to get a list element in the music categolry
  fitMedia(bass[index], 2, i, i+1)
  fitMedia(breaks[index], 3, i, i+1)

	
#default music in the back ground to add beats
fitMedia(HIPHOP_DUSTYGROOVE_001, 4, 1, 9)
fitMedia(HIPHOP_BASSSUB_001, 5, 1, 9)

#effect
setEffect(2,VOLUME,GAIN,10,1,-40,8)#lowers the music clip at track 2 and 3
setEffect(3,VOLUME,GAIN,10,1,-40,8)
#Finish
finish()
```
(There is no clip of the music since it is randomized, there is no point of putting one.)<br>
The above code would play a different set of music every time it runs. It would pick from the array of music in ``music``,``bass`` and ``breaks``. It does this by running the ``randint`` function to get a randomized number from 0 - 4 and then picks the element from the array using the number as the index value. Since the code is running on a loop, each time it runs it would run the loop 8 times to make 9 measure worth of music. Then it groups it together to create the music.
___
# Takeways
1.**Stop, research**. While working on this project I did not really understand how to make good music. What beat to use, what bass to use, breaks or snare. Until this point, I have been just sitting there and listen to every piece of music there is and if it sounds good I will use it. That was very inefficient so I took some time out of coding to learn a little bit about how to make music the general gist of things. It was worth it. I learned things like using beats and claps, using your breaks to move from one sound to the next. It really paid out.