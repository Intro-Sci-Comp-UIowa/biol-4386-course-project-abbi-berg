# Light intensity induces homosexual like courtship behavior in Drosphila Melanogaster

## Introduction
Courtship behaviors between male and female drosophila have been
extensively studied, however more recently, courtship behaviors between only 
male drosophila have been discovered and the factors that influence this 
behavior is the subject of our study. Traditionally, in order to engage in 
courtship with a female, a male drosophila must perform a courtship ritual to 
entice the female. The male will first begin this ritual by orienting 
themselves in the direction of the female and will chase the female around. 
Next the male fly will tap the female flys abdomen then extend its wing out and vibrate 
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
influences the presence of these behaviors, specifically we have found that 
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

### Figure to reproduce
For the purposes of this project, would like to produce a figure that is 
effective at displaying how increasing light intensity increases the frequency 
of male-male courtship behavior in drosophila, whereas male female courtship 
frequency is much less effected by the intensity of light.

I will plan to reproduce a modified version of Figure 1 from Lumley, 
Michalczyk, et al. 

![image](https://user-images.githubusercontent.com/78931288/111090280-35d9f180-84fd-11eb-9421-81b5c378c061.png)

Figure one. A line graph with distribution error bars at each point. For this projects 
purposes, the actual information presented in this graph is less relevent than the 
format of the figure itself. I would like to modify a version of this figure so that
points on the line would represent the frequency of each courtship event. The X axis would
in turn represent each time point (total 48 time points) with the light intensity increasing
each 12 points. One line would then represent the trials of only male flies and the other 
would be of trial with both males and females present. The error bars would represent the 
standard deviation. 


## Materials and Methods

### Data defined
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

### Method to produce figure

I will use preexisting data that indicates the presence of a courtship 
event at 96 intervals (12 intervals for each 2 min. light intensity 
period) to find the average number of occurrences of the 10 videos. 
I will also find the top and bottom 25 percentile range. The averages
and corresponding s.e.m. lines will be plotted on a line graph. Figure 
1 from Lumley, Michalczyk, et al, describes how I intend this to look.

See the drawing bellow for reference on how I intend to apply above line-graph 
technique for my purposes…

<img width="337" alt="image" src="https://user-images.githubusercontent.com/78931288/111090324-5ace6480-84fd-11eb-8a77-a23e712b8ab3.png">
 
The plotting of mean number of courtship events at each time will be
done in a seperate plot for each courtship event. Figure A then 
would represent wing extension events, Figure B chasing events and 
Figure C chaining events. 
 
I will then need to add color to the background of the graph to show the 
intensity of light increases every 2 min. Light intensity begins at 400 lux 
then increases to 700 lux, 14,000 lux and finially 17,000 lux.

I will use R for the statistical anaylsis of the data and for the creation
of the graph, however I am unfamilar with R studio, so I am unsure the
steps of this process. 

I would also like to explore an addition pannel that would allow me to quan-
tify the divergence between male and female behavior. This additonal graph wou-
ld show how the male courtship inceases with increasing light intensity while
male female courtship shows no difference. 

Please also update the Materials and Methods section with the relevant details for producing the figure. 

## Reflections

### Homework 1

From my homework 1 feedback, I was made aware that my description of the 
intensity of light was unclear. I addressed this by adding the specific 
light measurements to my introduction. It was also suggested that I add a 
fourth plot to show differences in male-male and male-female courtship. 
This would help illustrate that the light intensity effects male-male 
courtship more significantly than it effect male-female courtship. This 
is a great idea. My only concern is that while my data shows the intense 
light has a greater effect on male-male courtship than male female courtship, 
I am not sure to what magnitude. Also, male-male directed courtship is 
included in the male-female quantification of behavior because when counting 
the presence of each behavior it is difficult to distinguish if the behavior 
what sex the behavior was directed towards. I still would like to explore 
this more.

### Homework 2 
I recieved feedback from my homework 2 that I needed to fix my data format so it could be better read using R studio. I simplified the columns by removing the 'Lux' column and added the information to the rows containing the wing extension, chaining or chasing specification. I removed the white space as well and the columns that had totals and difference information. After taking the time to better understand my data and how R studio works, I definately think I need help continuing to format my data so that I can use it with ggplot. I also am realising that I need to refomat my figure to reproduce. I think that a box plot would be better than the line plot that I initially proposed. The data that I need to create a line plot like I initially imagined is not in the .csv file I added. I think that the boxplot format would be much more simplified than the line plot. 

![image](https://user-images.githubusercontent.com/78931288/114343361-5197de00-9b23-11eb-82b0-c4f61f02b83c.png)
Here is how I am thinking the box plot format would look. 

My feedback also suggested that I think about adding another figure to demonstrate how some behaviors may be greater effected by the presence of intense light by comparing the difference between the male only and male female trials. I think this would still be something to consider dispite that I am altering the type of plot that I will use. I still think that another plot that measures the difference between the previous light step and the next light step would be something to consider. 
See below
![image](https://user-images.githubusercontent.com/78931288/114344265-1e564e80-9b25-11eb-9fb3-ddb71789ab05.png)

Maybe something like this could be overlayed ontop of the boxplots. First order of buisness, I need to better understand how I need to format my data so that I can create a boxplot using ggplot. 

## Results 
you will show a preliminary figure or table. This can be a panel of a complex figure, or a crude plot that is starting to look like the final form. Provide the legend and some text description for the figure as you would find in a publication. 
-whats next
I have been stuggling trying to format my data. I have spent the last week trying to format data that could be used to make the line plot I initially suggested for use in R studio and I think that it is too complex and that the data I already have updated and now reformated will be better to use. So far in R studio I have created a markdown file to keep track of the code I am using to produce my figure. 

So far what I have done is uploaded my .csv file to R studio using the read_csv function. Unfortunately this is as far as I have gotten. I am really struggling to figure how to tell ggplot what I want as my X and Y varriables for the plot. I want on the x axis in this order... MM 400 lux chasing, MF 400 lux chasing, MM 600 lux chasing, MF 600 lux chasing, MM 1200 lux chasing, MF 1200 chasing, MM 17,000 lux chasing, MF 17,000 chasing. On the Y axis I don't want a particular column of data, but the numbers underneith the columns listed. This is truely step one for me. After this then I can assign colors to each box (pink to symbolize MF trials and blue to symbolize MM trials). After I finish this very important step, then I might consider overlaying lines like the ones drawn above to show the difference between the light steps. 

## Discussion
 Ultimately I think that I didn't understand what data I had. The data I have been uploading does not contain the specific timepoints, but rather it has the total number of times a certain behavior occured out of 12 total possible times at each light intensity. I think that using this synthesized data is better 1) because I already have it uploaded and 2) because the formating is closer to being ready for use by ggplot than the alternative. After I realised that the data I had uploaded and the data I would need for my figure was different, I attempted to format the alternative data to use in R studio and I could not figure a good way to use and manipulate it with R.  
