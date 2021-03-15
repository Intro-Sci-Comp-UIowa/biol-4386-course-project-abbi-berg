# Light Intensity Induces Homosexual Courtship in Drosphila

## Introduction
Courtship behaviors and rituals between male and female drosophila have been
extensively studied, however more recently, courtship behaviors between only 
male drosophila have been discovered and the factors that influence this 
behavior is the subject of our study. Traditionally, in order to engage in 
courtship with a female, a male drosophila must perform a courtship ritual to 
entice the female. The male will first begin this ritual by orienting 
themselves in the direction of the female and will chase the female around. 
Next the male fly will tap the female fly then extend its wing out and vibrate 
it to produce a courtship song. The final step in courtship before copulation 
is that the male will lick the genitalia of the female. If all goes well the 
end result will be copulation between the sexes. Some of these courtship 
behaviors have been found to exist even in male only populations. Most 
interestingly, male drosophila will orient themselves to one another and chase 
each other around so that they from chains and sometimes even loops of male 
flies. Male flies will also extend their wing and produce a courtship song 
even when no females are present.

It is unknown why male drosophila would perform these courtship specific 
behaviors when females are not present. In my lab we are studying what 
influences the intensity of these behaviors, specifically we have found that 
male-male drosophila courtship behaviors become more frequent when the 
intensity of white light is increased with the most courtship behavior 
occuring at 17,000 lux white light. We have observed this by placing male 
drosophila in flat ‘arenas’ in which the courtship behaviors (specifically the 
wing extension, chasing, and chaining behaviors) are observed and the frequency 
of these behaviors is noted. We are able to use LED lighting that can be made 
more or less intense to then observe the frequency of behavior. A control 
experiment is also done including equal parts male and female flies and light 
intensity has shown to have less effect on the frequency of courtship between males 
and females. 

## Figure to reproduce
For the purposes of this project, would like to produce a figure that is 
effective at displaying how increasing light intensity increases the frequency 
of male-male courtship behavior in drosophila, whereas male female courtship 
frequency is much less effected by the intensity of light.

I will plan to reproduce a modified version of Figure 1 from Lumley, 
Michalczyk, et al. 

![image](https://user-images.githubusercontent.com/78931288/111090280-35d9f180-84fd-11eb-9421-81b5c378c061.png)
Figure one is a line graph with distribution error bars at
each point. 

My data is as follows: 8 minute videos of male-male and male-female trails have 
been taken. Every 2 minutes throughout the video, the light intensity is 
increases. The presence of a wing extension, chasing or chaining event is 
recorded 12 times throughout each 2 min. light interval. Ten 8 min. videos 
have been recorded. I would like to produce three figures for each courtship 
event (wing extension, chasing and chaining). For each event I would like to 
produce something that looks similar to the above in which the red line would 
represent the male-female trial and the blue would represent the male only 
trial. On the X-axis would be the time elapsed and the Y-axis would be called 
the frequency of each particular courtship event. Each point on the graph 
would be the average number of times the courtship event was observed of the 
total 10 videos with 1.0 being that the event was observed in all of the videos 
within the interval of time. There would be 12 total intervals for each 2 min. 
period of time. 

See the drawing bellow for reference on how I intend to apply above line-graph 
technique for my purposes…

<img width="337" alt="image" src="https://user-images.githubusercontent.com/78931288/111090324-5ace6480-84fd-11eb-8a77-a23e712b8ab3.png">

I would also like to highlight each 2 min. section of the line graph with an 
increasing shade of color to indicate that the intensity of light is 
increasing in each 2 min. time period. Figure A then would represent wing 
extension events, Figure B chasing events and Figure C chaining events. Like 
in the Figure 1 from Lumley, Michalczyk, et al, I would also like to add 
s.e.m. lines like to each point that would represent the top 25th percentile of 
the time and bottom 25th percentile to each point.

## Steps to produce figure
1. I will use preexisting data that indicates the presence of a courtship 
event at 96 intervals (12 intervals for each 2 min. light intensity 
period) to find the average number of occurrences of the 10 videos. 
I will also find the top and bottom 25 percentile range.
 
2. I will then need to plot the averages for the male only and male-female 
trial. I will need to add error bars for each of the points.
 
3. I will then need to add color to the background of the graph to show the 
intensity of light increases every 2 min. Light intensity begins at 400 lux 
then increases to 700 lux, 14,000 lux and finially 17,000 lux.

4. I will use R for the statistical anaylsis of the data and for the creation
of the graph. 

5. I would also like to explore an addition pannel that would allow me to quan-
tify the divergence between male and female behavior. This additonal graph wou-
ld show how the male courtship inceases with increasing light intensity while
male female courtship shows no difference.
