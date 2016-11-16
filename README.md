# P6_Data_Visualization_1
## Summary - 
Titanic dataset contains demographics and passenger information from a subset of the 2224 passengers and crew on board the Titanic. 
I aggregated the data into age groups and calculated the max,avg and min of fare for survived and perished in each age group. 
The data set is to discover the positive correlation of meanfare and survival, except for children under 10years old and old people of 
70s and 80s, who depended more on their families. Overall, passengers with higher fares were more likely to survive.

## Design - 
I'd like to examine the relationship of socialeconomy variables and survival. So I select fare as socialeconomy variable. 
In order to show clear pattern across different ages. I aggregated age to groups and calculate fare for each group of survived and perished. 
At first, I select bar chart because bar chart is very appropriate for observing the comparasion of mean fare. I colored the survived with green and perished with red. 
Here's my first version: http://bl.ocks.org/Maggiebj/57d03dc2b8819d532ae2201d791c1afe
Followed first feedback, The major revision in second version is adding summary statistis summary of min, 25%, mean, median, 75% and max to the plot.
Here's my second version: http://bl.ocks.org/Maggiebj/99852d12304e0c8090cf59582491e8bb
Followed the second and third feedback, I revised the plot by showing summary of fare in one plot,and switch plots by each age group.
Here's my third version: http://bl.ocks.org/Maggiebj/29bd0a199629d1fba11a37327b2206e0

## Feedback -
###From Myles (Forum Mentor),feedback for the first version:
1.What do you notice in the visualization? 
As the commentary suggest, for each age group (except under 10s) the mean fare is higher for the group that survives than those who perished. 
2.What questions do you have about the data? 
Some summary statistics may be an interesting addition to the commentary (how many in each category, for example, and information about the fares). 
3.What relationships do you notice? 
As stated, a clear relationship between mean fare and survival category. 
4.What do you think is the main takeaway from this visualization? 
As above. 
5.Is there something you don’t understand in the graphic? 
It may be nice to see the distribution of fares (as I noted above). Are the mean fares skewed by some large fare values? The same graph with median fares would be a nice comparison. 

###From georgeliu1998 (Forum Mentor), feedback for the second version:
Great work! I like how you used the legend for filtering and interaction. Also, the title clearly conveys your main finding. That said, I do have a different angle for you to consider:
It took some time for me to figure out what the top left buttons do. It turns out they allow the switching among different metrics for the y-axis. Also the legend based filtering doesn't seem to add much to the insight being communicated. Furthermore, when your main finding is about the full cohort of passengers instead of a single group, it may be a little overwhelming to present all the data for all age groups at first sight.
To address the above, you can consider doing this:
Use a box plot to show a fuller picture of the comparison of the full spectrum of distribution. This way, you don't need the top buttons. Also, present one big boxplot comparing survival vs. not, and present the option of different age groups using buttons so that people can further explore if they wish.

###From Andy (DAND student), feedback for the second version:
It is confusing to show quantile data in different plot, it may be better to show statistic summary in one plot. Should the age group in button be better?

## Resources - 
some dimple and d3 examples and documents: 
http://dimplejs.org/advanced_examples_viewer.html?id=advanced_interactive_legends 
https://github.com/PMSI-AlignAlytics/dimple/wiki/dimple.axis#properties-1
https://github.com/d3/d3/blob/master/API.md#arrays-d3-array
https://discussions.udacity.com
