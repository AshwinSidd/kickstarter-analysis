# kickstarting with Excel
## Overview of the project 
The aim of the project was to help an upcoming playwriter Louise, crowd fund her play *Fever*. The estimated budget was $10000. Using the Kickstarter Data that was given, the aim was to check how other crowd funded campaigns fared in relation to their goals and time (launch date).
## Purpose
The purpose of the project was to **analyze** the dataset, **visualize** how other campaigns fared by analyzing outcomes based on launch dates and goals set, which would then help Louise better understand her approach towards her campaign.  
## Analysis and Challenges
The approach was to first analyze the outcomes of other campaigns based on their launch date, then to visualize outcomes based on their goals. This would give Louise an understanding what period is best to launch her play and with what budget estimate. 

For the first part of analyzing the *outcomes by launch date*, it was important to change the Unix timestamps on the launch dates of the data set. Hence a date conversion formula was applied to it, and then since we also wanted to analyse the data w.r.t the year, the year fomula was applied to the date conversion column. The below screenshot shows the data being cleaned - **Date created conversion** from Unix and then formulating the corresponding **Year**.

![Data date conversion](https://user-images.githubusercontent.com/92342751/139591111-62614f0d-f9ec-4045-8505-5952dd41a12a.png)

Next, a pivot table was created using the count of outcomes as the value corrsponding to the launch date (converted from Unix timestamp), this was also filtered using years and the parent category which was filtered to Theatre on the pivot table. *A line chart* was then created using this data, which gave us a visual analysis of how the plays fared in relation to their launch dates. Below is the **pivot table**. 

![Pivot chart](https://user-images.githubusercontent.com/92342751/139592565-7b717ef5-1697-45b6-a9c1-ddfaeb51e45d.png)

For the second part to *analyze outcomes based on goals*, a seperate excel sheet was created to see how the plays fared based on parameters. The parameters were the goal amounts put into bins of equal ascencions of $5000, starting with any value lesser than 1000 and ending with any goals reached which were greater than $50000. Then the **Countifs** formula was applied to see how many count of plays corresponded to being *succesful, failed or canceled*. From these, a perecentage for each of the category was found out.

![Countifs](https://user-images.githubusercontent.com/92342751/139591478-aa3dce54-0324-4c95-b06b-e9e547c5658c.png)

From the above table, a line chart was created which is explained in the later part of this analysis. 

**The challenges** with the data set was that, while it was an extensive data which was raw, unflitered or uncleaned. To start with the data set had to be cleaned, some of them had no values, which would hinder the use of formulae in excel. The timestamps were in Unix too, hence had to be converted. Data had to be filtered and made sure that only the data required for the outcome of the play was used. 

## Analysis of outcomes based on launch date
Based on the analysis, where we compared which months the plays fared better (had more relative successes), the line chart clearly shows a **peak in the months of May and June**. Which means that of May had the most susccesful campaign outcomes. The month of June came second, relatively closed to May. So the month of May would be the optimal/preferred time for Louise to launch the campaign. Having said that the month of months of June, July and October had relatively more failures. Louise needs to be vary about this and could surely avoid the months of October and July to launch.

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/92342751/139592493-b0e9c7c4-d6b0-4e33-8317-bb206c3a42bb.png)

## Analysis of Outcomes based on Goals
Based on this analysis, it was seen that all campaigns with a goal of less than $1000 fared succesfully, followed closely by the ones between $1000 to $4999. The danger goal amounts seem to be the ones between 25000 to 29999,30000 to 34999 and the only 1 campaign in the 45000 to 49999 range failed too.

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/92342751/139592498-1b933203-a539-477d-8d10-d4851b8a997d.png)

## Challenges and difficulties encountered
With a large data set, the challenge is to ensure that the right data is used to calculate and derive the analysis required. Understanding which data had to be worked on and the direction to take was another key aspect. The launch date analysis was simple, the formula was easy. However, the challenge or difficulty was when analyzing the outcomes based on goals - each formula for the corresponding goal parameter set had to be typed accurately. I faced difficulty in the line graph outcome as it did not match with what it was supposed to look like. I had to play around and re-worked the sheet multiple times to see if there was an error with the formuale or the data set. Finally the attempts paid off. 
## Results
For outcomes based on launch dates, it is clear that May is the best time to launch the play as the probability of the play succeeding is higher. October relatively seems to be the month with higher rates of failures relative to the total number of plays. 
For outcomes based on goals, the ideal goal target could be $5000 as a lot of succesful plays had this goal. Since Louise planned her goals to be $10000, we could advice her that the target had lesser percentage of success compared to any goal lesser than $5000

There however, are some *limitiations* to this data set. The data set does not account for the "qualitative" aspect of the plays. To be precise, plays with a better cast may be the reason for its succes. If data for "reviews" were available fo reach of the plays, that would have been a good measure to understand the data better. With the curent data available, there are a couple of outliers that need to be considered. A Box and Whisker plot would give us the outliers which could help us analyze the data set better. A percentage average of the outcomes by launch dates may give us more information based on the overall campaign outcomes. 

*Other charts* can also be used to analyze the data. For the outcomes by goals, a column graph helps in comparing the campaign outcomes closesly. I have used column graph for both analysis of outcomes by launch dates (filtered for succesful campaigns) and for outcomes by goals. Below 2 screenshots give a good picture too - 

![Bar chart 1](https://user-images.githubusercontent.com/92342751/139593186-fad7b8b7-baac-4b9f-8214-d0e9cfe3fee7.png)

![Bar chart 2](https://user-images.githubusercontent.com/92342751/139593257-947c0aea-df31-40e8-adcb-3401a24faa7c.png)

I also used a pie chart to view the Failed outcomes based on goals vs the succesful outcomes based on goals. It also gives me a good picture of how the campaigns failed and succeeded across the goals.

![Pie chart 1](https://user-images.githubusercontent.com/92342751/139593508-919520da-3e53-476c-97a2-ab488705661e.png)

![Pie chart 2](https://user-images.githubusercontent.com/92342751/139593512-4f713cb9-434e-4299-a8c6-54ae8c570086.png)




