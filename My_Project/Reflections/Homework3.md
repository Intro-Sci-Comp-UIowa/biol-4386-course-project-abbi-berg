# Deciding to change to boxplot
I recieved feedback from my homework 2 that I needed to fix my data format so it could be better read 
using R studio. I simplified the columns by removing the 'Lux' column and added the information to the 
rows containing the wing extension, chaining or chasing specification. I removed the white space as well 
and the columns that had totals and difference information. After taking the time to better understand my 
data and how R studio works, I definately think I need help continuing to format my data so that I can 
use it with ggplot. I also am realising that I need to refomat my figure to reproduce. I think that a box 
plot would be better than the line plot that I initially proposed. The data that I need to create a line 
plot like I initially imagined is not in the .csv file I added. I think that the boxplot format would be 
much more simplified than the line plot.

image Here is how I am thinking the box plot format would look.
<img width="739" alt="image" src="https://user-images.githubusercontent.com/78931288/117244218-42444180-adfe-11eb-8b91-b8a42bf943c7.png">


My feedback also suggested that I think about adding another figure to demonstrate how some behaviors may 
be greater effected by the presence of intense light by comparing the difference between the male only and 
male female trials. I think this would still be something to consider dispite that I am altering the type 
of plot that I will use. I still think that another plot that measures the difference between the previous 
light step and the next light step would be something to consider. See below image
<img width="739" alt="image" src="https://user-images.githubusercontent.com/78931288/117244186-35275280-adfe-11eb-9965-cd2479d0b0a7.png">


Maybe something like this could be overlayed ontop of the boxplots. First order of buisness, I need to better 
understand how I need to format my data so that I can create a boxplot using ggplot.

# Results

I have been stuggling trying to format my data. I have spent the last week trying to format data that could 
be used to make the line plot I initially suggested for use in R studio and I think that it is too complex and 
that the data I already have updated and now reformated will be better to use. So far in R studio I have 
created a markdown file to keep track of the code I am using to produce my figure.

So far what I have done is uploaded my .csv file to R studio using the read_csv function. Unfortunately this 
is as far as I have gotten. I am really struggling to figure how to tell ggplot what I want as my X and Y 
varriables for the plot. I want on the x axis in this order... MM 400 lux chasing, MF 400 lux chasing, MM 
600 lux chasing, MF 600 lux chasing, MM 1200 lux chasing, MF 1200 chasing, MM 17,000 lux chasing, MF 17,000 
chasing. On the Y axis I don't want a particular column of data, but the numbers underneith the columns listed. 
This is truely step one for me. After this then I can assign colors to each box (pink to symbolize MF trials 
and blue to symbolize MM trials). After I finish this very important step, then I might consider overlaying 
lines like the ones drawn above to show the difference between the light steps.

# Discussion

Ultimately I think that I didn't understand what data I had. The data I have been uploading does not contain 
the specific timepoints, but rather it has the total number of times a certain behavior occured out of 12 total 
possible times at each light intensity. I think that using this synthesized data is better 1) because I already 
have it uploaded and 2) because the formating is closer to being ready for use by ggplot than the alternative. 
After I realised that the data I had uploaded and the data I would need for my figure was different, I attempted 
to format the alternative data to use in R studio and I could not figure a good way to use and manipulate it with R.
