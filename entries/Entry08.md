# Entry 8: Starting final project
For my final project, I have planed on making a music that I myself would consider to be good. Something that is not just ok but an improvement compared to the previous music I have made. A piece of music I will be willing to share to others because it is a good beat or something I am proud to post online.  

```python
from earsketch import *
from random import *
init()
setTempo(145)

for i in range(1,5):
  fitMedia(DUBSTEP_LEAD_020,3,i+4,10)#this creates a intresting interaction where the music overlap itself. Making a new sound.

for i in range(1,10): 
  makeBeat(OS_KICK03,5,i+3,"00--00----000-00")#drum beat in the background needs to be loop for efficiency

#body of the music
fitMedia(DUBSTEP_LEAD_001,1,1,3)
fitMedia(DUBSTEP_LEAD_004,2,3,4)
fitMedia(DUBSTEP_LEAD_004,2,4,5)
fitMedia(HIPHOP_STOMP_BEAT_PART_005,4,5,11)
fitMedia(YG_WEST_COAST_HIP_HOP_CLAP_SNARE_1,4,4,11)
fitMedia(RD_FUTURE_DUBSTEP_SUBBASS_7,6,10,14)
fitMedia(RD_TRAP_SOFTBELLLEAD_1,7,7,7.5)
fitMedia(RD_TRAP_SOFTBELLLEAD_1,7,7.5,8)
fitMedia(RD_FUTURE_DUBSTEP_FILL_5,8,10,14)
fitMedia(RD_FUTURE_DUBSTEP_FILL_2,8,10.5,14)
  
#effects, some of them are placeholder at the moment
setEffect(1,VOLUME,GAIN,-10,1,-10,14)
setEffect(2,VOLUME,GAIN,-20,1,-50,14)
setEffect(3,VOLUME,GAIN,-20,1,-20,14)
setEffect(4,VOLUME,GAIN,-15,1,-15,14)
setEffect(5,VOLUME,GAIN,-20,1,-40,14)
setEffect(6,VOLUME,GAIN,-20,1,-20,14)
setEffect(7,VOLUME,GAIN,-5,1,-5,14)
setEffect(9,VOLUME,GAIN,-20,1,-15,14)
finish()
```
[listen to the music HERE](https://clyp.it/vuesrojt)<br>
After a whole week of tinkering and a couple hours over the weekend. I realized that I was trying too hard to fit randomness into my project. Due to the fact that if the music is random it is harder to create something that is good to listen to. I would have to make sure that every random possibility of the music needs to sound good. That is just too much for me and would require me to have a wayyyyyyyyyy deeper understanding about how to make beats and mixing. I am just a beginner when it comes to music production and I was trying too hard to make something that was out of my league.

---
# Takeways
1. **Don't try to do too much.** Understand your own limits and go build from there. This refers back to Mr.Mueller's MVP where you have to start from the simplest project first and slowly build upon that project to have more and more functions. You can not start building a house with a roof. You have to start with the basics, the foundation.
2. **Don't force it** Like I said in my entry I was trying too hard to force randomness into my music and it end up with me wasting all my class time. Where I was constantly listening to the music and see if each combination of the music sounds well together. And during the week I had the though that this might not work out but I did not want to give it up. I know that I can make it happen. But I should have realized it sooner that just because I know eventually I can make it happen does not mean it will. Persistence is a good trait to have but in this case, it has hurt me more than it has helped.