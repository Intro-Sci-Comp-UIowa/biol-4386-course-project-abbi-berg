# Light intensity induces male-male courtship behavior in *Drosphila*

This repo was created in Spring of 2021 for the class BIOL:4386 taught by Bin He. It outlines the process 
to produce a figure that displays how male-male courship behavior in *Drosophila* can be induced with intense 
light. 

### File organization reference guide
| Directory | Notes |
| --- | --- | 
| Data/ | contains data files to produce figure; all data used in R markdown files can be found here |
| Output/ | pictures of the figures produced using R studio; R code can be found in R markdown files |
| Reflections/ | feedback and evolution of thought and theory behind figure production; contains homeworks 0-3 |
| Script/ | contains R markdown files used to produce figures |


## Introduction
Courtship behaviors between male and female *Drosophila* have been
extensively studied (Hall, 1994), however courtship behaviors between only 
male drosophila have also been observed (McRoberts & Tompkins, 1988) and the factors that influence this 
behavior is the subject of this study. Traditionally, for male *Drosophila* to engage in 
courtship with a female, a male *Drosophila* must perform a courtship ritual. The male's ritual begins
with the male orienting itself to the female. Next the male will chase the female around, 
tap the female fly's abdomen and then extend its wing out and vibrate 
it to produce a courtship song. The final step in courtship ritual before copulation 
is that the male will lick the genitalia of the female (Hall, 1994). Some of these courtship 
behaviors have been found to exist even in male only populations. Most 
interestingly, male drosophila will orient themselves to one another and chase 
each other around so that they form chains and sometimes even loops of male 
flies. Male flies will also extend their wing and produce a courtship song 
even when no females are present.

It is unknown why male drosophila would perform these courtship specific 
behaviors when females are not present. Data exists that indicates that 
male-male *Drosophila* courtship behaviors become more frequent when the 
intensity of white light is increased. For the purposes of this project, a figure
was produced using this data. Though this was not the initial intent of the project, 
after realizing the limitations of the data as well as workshoping multiple 
methods of displaying the data, a final bar and scatter plot figure was produced. 

## Methods

### Data collection
The goal of the project was to produce a figure that displayed how intense light can induce 
male-male courtship in *Drosophila*. The data used to produce this figure was collected
by members of the Dr. Wu lab at the University of Iowa. *Drosophila* were exposed to four different 
intensities of light: 400 lux, 2,000 lux, 6,000 lux, and 17,000 lux. There were three courtship 
behaviors observed: wing extensions, chasing, and chaining. Eight male flies were kept in 
a chamber and exposed to each light intensity for 2 minutes each starting with the lowest light
setting then gradually increasing to the most intense light setting. The observer would watch 
the chamber of flies for 5 seconds and record if each behavior occurred. The 5 second observation 
period was then followed by 5 seconds of no observations and then this on and off period was
repeated 12 times for each light intensity. The total number of times a courtship 
behavior could occur was 12 per chamber per light intensity setting. Observers then counted the 
total number of times each event happened for each chamber and recorded it. This process was also
done using four males and four virgin female flies as a control. 20 chambers total were observed. 
This record can be found in the Data/ dirrectory and is labled 04112021_LightProtocol_shortformat.csv.

### Figure production
**Figure 1. Pipeline for the production of figure**

<img width="630" alt="image" src="https://user-images.githubusercontent.com/78931288/117385513-e7b4ef00-aeaa-11eb-81e5-1ee2fd290dad.png">

The pipeline used to produce the figure changed throughout the duration of the class. Initially, 
it was thought that the data collected would be ready as is for use by plyr and ggplot in R
Studio (figure 1, a), however the data needed to be converted to long format to be understood 
by R Studio. Tidyverse was used to convert the wide format original data to the long data format. 

Originally it was thought that the data would be visualized using a line graph, however a better 
understanding of the data lead to the exploration of other methods that would better convey that
increasing light intensity increases the presence of male-male courtship in *Drosophila* and 
therefore a more accurate pipeline of how the final figure was produced was rendered (figure 1, b).

**Figure 2. Initial idea for data visualization**

<img width="874" alt="image" src="https://user-images.githubusercontent.com/78931288/117383138-aa019780-aea5-11eb-8afa-c43c98bc7cb5.png">

> Line graph figure was taken from Lumley, Michalczyk, et al. and annotated to demonstrate how the authors figure concept would be used with *Drosophila* light intensity data. 
>> Lumley, A., Michalczyk, Ł., Kitson, J. et al. Sexual selection protects against extinction. Nature 522, 470–473 (2015). https://doi.org/10.1038/nature14419

The initial model used to envision the concept for the final figure was taken from Lumley, 
Michalczyk, et al. The concept was to produce a line graph which plots the proportion of chambers
in which a specific courtship behavior was present at each of the 12 time points (figure 2). Recall 
that each chamber was exposed to four light intensity settings and that within each intensity, 
12 time points were recorded. The total number of time point then to be represented on the X-axis 
would be 48. This was determined to be an excessive amount of information to plot. The goal of the 
figure was to display how with each increase in light intensity, the courtship activity frequency 
increased, therefore displaying the frequency of each courtship event at each timepoint of each light
intensity was unnecessary to serve its purpose. In addition to this method being excessive in its 
format, the data used to create the figure was also insufficient since it contained the total 
number of each courtship event at each light intensity and lacked information about each 
individual time point within each light intensity. Raw data sheets exist that show each timepoints
information, but are not compiled nor uploaded to this github repository. 

**Figure 3. Boxplot and scatterplot draft**

<img width="544" alt="image" src="https://user-images.githubusercontent.com/78931288/117383307-1aa8b400-aea6-11eb-8b75-c64515a6bb9d.png">

Since it was determined that summarizing the frequency of courtship events at each light intensity would be
better at serving the figures purpose, a box plot and scatter plot design was drafted using ggplot to present the 
light intensity data (figure 3). This method displayed the necessary information to show how
intense light increases the presence of male-male courtship behavior and avoided having confusing excess
data points. A scatter plot was determined to be essential since it preserved each individual
chambers data and helped to display the spread of the data, though having a both a boxplot and a scatterplot
was redundant. 

**Figure 4. Male-male courtship behavior is induced by intense light**

<img width="866" alt="image" src="https://user-images.githubusercontent.com/78931288/117383371-4461db00-aea6-11eb-8651-8a7297053b01.png">

Finally it was settled that a bar graph to plot the mean frequency of all the chambers data would be the
best way to display the courtship behavior. This method supported the consolidated use of both the raw data
as well as easy to read summarized data all in one figure. The bar graph helps the reader to visualize the trends
of the raw data in an easy to understand format. The bar graph was also coupled with lines to display the standard 
deviation. 

## Results
As the light intensity increased, the frequency of all courtship behaviors increased. 
This was true for chambers containing only males as well as for chambers containing 
both males and females, however the increase in behavior was more dramatic in the male 
only chambers than in the chambers containing both males and females (figure 4). The 
frequency of behavior at low light intensity was higher in chambers containing both 
sexes and male-male courtship behaviors were nearly nonexistent at the lowest light 
setting (400 lux). Chaining behaviors were nearly absent in all light intensities except 
the highest light intensity (17,000 lux). In both male only chambers as well as in chambers
with both sexes this chaining behavior was present at similar frequencies. It should be noted
that chaining behavior was recorded if at least four *Drosophila* were chasing one another
in an unbroken chain. In chambers containing both sexes, this could result from all 
four males chasing one another or from three males chasing behind one female. Females
were not seen chasing other male or female flies. 

## Discussion and Conclusion
Though the initial concept for the figure was abandoned for the bar graph and scatter
plot method, the progression of the figure lead to a clearer display of the data's concept. 
The final figure is less redundant and more simplified therefore, it is easier for the
viewer to comprehend the point that intense light increases the presence of male-male
courtship in *Drosophila*. 

The figure also highlights how male *Drosophila* will continue to perform male-male 
courtship behavior even in the presence of females. The male *Drosophila* will choose 
to chase another male *Drosophila* even when equal parts of males and females are present. 
In some cases all males would be chaining behind a single female though other females were
available. It could be possible that one particular female was preferred by all males and therefore
all males sought to court the same female at once. It was seen that the males when in 
chains behind a single female would switch positions in the chain. A potential hypothesis 
for the presence of this male-male courtship could be that it acts a mechanism for which 
male *Drosophila* compete for an optimal female, though this data is not in itself 
sufficient to support this. To further analyse this hypothesis, the knowledge that 
high light intensity increases the frequency of male-male courtship behavior would be of 
use. Intense light can act as a mechanism to induce male-male courtship behavior which can 
further help aid in the quest to reason why male *Drosophila* will court other male *Drosophila*
even when seemingly their energy may be better spent courting female *Drosophila*.

## Reflection
I was very surprised at how difficult it was for me to simply produce any figure in 
R Studio using my data. For the longest time I was convinced I was using the ggplot
function incorrectly, however when I learned I needed to convert my data from wide 
format to long format, my challenges producing a plot were much better understood.
Producing my first boxplot using my data was certainly a high point for me in the project.
I think the biggest take away I have from this project is that I now have a better
understanding of how data must be formatted for use by programs such as R. I think 
that also the process of workshopping my figure and developing it to further serve 
my purpose forced me to learn many graphing functions in ggplot which I can now use 
for future projects. I really feel that I would've been much better off having had
the knowledge of how to visualize data in R earlier in my undergraduate career. In 
past projects and lab reports I always struggled using Microsoft to produce figures 
because I would often have ideas for the graph that Excel did not have the functionality
to do. 

Another skill I much appreciate learning from this project is how to use R Markdown files.
I really love how you can annotate and section code in markdown. I think this 
function is a very useful tool that promotes reproducibility as it allows you to
really spell out why certain code is used. I know that for my purposes, from this 
project I now have a reliable R Markdown file that I can make small modifications
to to visualize other data sets. I know that if I came back to this project in 
a couple years, that using my markdown file I would be able to understand how the
figure was produced. 

This method of documenting and managing projects using GitHub was also new to 
me, but I feel that it is a very useful project management tool. I have implemented
a similar file organization system to the google drive that we use in my lab for
this project. Instead of README.md files, I created README.md style documents that 
help make navigating through the directory more user friendly. I like putting tables
that describe each file in the folder in those README.md files as they ensure
it is clear what is in the file and helps to prevent lost files. Since this project
I have also been more mindful of how to name files consistently and descriptively.

## References
Hall JC. The mating of a fly. Science. 1994 Jun 17;264(5166):1702-14. doi: 10.1126/science.8209251. PMID: 8209251.

McRobert, S., & Tompkins, L. (1988). Two Consequences of Homosexual Courtship Performed by Drosophila melanogaster and Drosophila affinis Males. Evolution, 42(5), 1093-1097. doi:10.2307/2408925

## Acknowledgements
The author would like to thank Professor He and Ethan for help troubleshooting technical difficulties as
well as the BIOL:4386 class members for sharing their computing skills. The book *Bioinformatics Data Skills* by 
Vince Buffalo was also used as a resource for this project. 

This author would also like to acknowledge Dr. Wu's lab at the University of Iowa for the resource to collect 
this data as well as both Dr.Wu and Dr. Ueda for their contribution to the development of the produced figure. 
Finally lab colleagues Madeline, Diandian and Shuwen will be acknowledged for their help collecting data. 

