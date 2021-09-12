# kickstarterproject

## Overview of Project
### Purpose
In search of insights to help inform current and potential future kickstarter project decisions, data from previous performing, visual, and musical arts kickstarter campaigns were analyzed for the client, Louise. Data include launch date, monetary goals, actual fundraising amounts, the outcome of the project (completed, failed, or canceled), country, etc..

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
In order to conduct this specific analysis, I was able to format the Unix launch date to a readable form using the formula (((A1/60)/60)/24)+DATE(1970,1,1) (A1 is a generic cell address for explanation purposes). Using the newly formatted data, I was able to create a pivot chart which tabulates the total numbers of failed, successful, and cancelled theater projects based on the month of their launch date, and created a corresponding line graph ![This is an Image](https://github.com/phillipbrock/kickstarterproject/blob/main/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based On Goals
For this analsysis, I categorized fundraising goals roughly based on $5000 increments, with a lower category of less than $1000. I then was able to tabulate which plays were successful, failed, and canceled using the COUNTIFS function to set criteria, and created a corresponding line graph ![this is an image](https://github.com/phillipbrock/kickstarterproject/blob/main/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered
While the data are wide-ranging, the client specifically is interested in insights into launch dates and funding goals. In order to make sense of the data, I was able to parse out categories and subcategories in order to give the client data that are most relevant to projects she is pursuing, in this case, theater. I also formatted the outcomes of the kickstarter campaigns so the differences between success, cancellation, and failure are easily digested. ![this is an image](https://github.com/phillipbrock/kickstarterproject/blob/main/formatting.PNG)  


I also formatted the percentage of fundraising on a color gradient, which makes it more intuitive to see how well each project performed in fundraising relative to the goal. ![this is an image](https://github.com/phillipbrock/kickstarterproject/blob/main/formattingfundraising.PNG)  


I am confident this analysis is accurate and insightful, though it did not come without challenges. Most notably, this dataset is extensive and much of the data were not particularly useful for the needs of the client. Organizing the data so that the analysis carried the most validity for the needs of the client was an obstacle, but was achieved by using pivot tables to filter based on the type of kickstarter (theater, and specifically plays, were more useful than music or television projects), as well as using sorting functions such as “COUNTIFS” to distil the data. Also, the large dataset makes it difficult to verify the accuracy of the use of such sorting tools. For example, while I am confident I correctly applied the “COUNTIFS” function, with over 4000 projects included in the dataset, verifying the output is not entirely feasible.
## Results
-  What are two conclusions you can draw about the Outcomes based on Launch Date?

According to these data, the most successful month to launch by number of successes has historically been May, though it also has been the most prolific month (so there are also the most number of failed projects). This analysis also shows that October and December have historically been the worst months for launch. This can be seen on the included graph which shows the number of failed and successful projects have been almost equal in those months.
- What can you conclude about the Outcomes based on Goals?

The analysis of outcomes based on fundraising goals shows that smaller projects with a goal of less than $1000 were the most successful. It also shows that goals between $35,000 and $45,000 were largely successful, though this is based on a much smaller sample size. It also shows that the majority of projects with goals between $20,000 and $35,000, or greater than $45,000 have historically shown to fail rather than succeed.
- What are the limitations of this dataset?

While this analysis is useful, it is limited in a number of ways. The conclusions for date of launch, for example, may be skewed by differences in geography. While it appears the summer months are the most favorable for theater kickstarters, are the majority of the projects based in the northern hemisphere? Would the trend be the opposite for clients in the southern hemisphere, where the seasons are reversed? For fundraising goals, do the most ambitious projects greater than $45,000 fail because they are too ambitious, or for some other qualitative reason such as the skill of the organizers or the locations of their projects? With smaller sample sizes for larger projects, such factors can be misleading in the data. Likewise, are so many smaller projects, like less than $1000 for their goal, not ambitious enough? With their high success rate, could some of these projects have set loftier goals and have a chance for a higher return?
- What are some other possible tables and/or graphs that we could create?

For further analysis, especially for date of launch, it would be useful if the data could be separated by northern and southern hemisphere to see if the trend described above holds true for both. The analyses described above are also unnecessarily difficult to digest in that they only compare the raw numbers of how many projects failed, were successful, or were canceled. This can cause confusion and be misleading for categories where there are higher successes, but also more failures because the overall number of projects are greater (like those launched in May, or those with a goal of less than $1000). What would be more helpful would be to graph the percentages of each, and compare them to an overall baseline. This way, one could clearly see which months, or fundraising goal categories, have shown the highest percentage of success regardless of how many actual projects are started in each. For example: ![this is an image](https://github.com/phillipbrock/kickstarterproject/blob/main/percentage.png)
