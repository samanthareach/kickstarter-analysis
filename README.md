# kickstarter-analysis
## Analysis
###### This project examined how different campaign's fared in relation to their launch dates and their funding goals. 

## Analysis and Challenges
###### In order to acquire this data, I created a "Years" column based on the "Date Created Conversion" column in the Kickstarter spreadsheet, using the "YEAR()" function. 

###### I created a pivot table based on the "Parent Category" and "Years" columns. I then filtered the "Parent Category" to only show the data for "Theater", and then sorted the campaign outcomes in descending order.  

###### To visually represent the data, I created a line chart that showed the number of successful, failed, and canceled projects by month. 

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/103145291/174222489-43aa86c9-9f6a-40d7-b694-537d7fb54144.png)

###### According to the graph above, May is the month with the most successful Kickstarter campaigns. May, June, July, and October all have a relatively similar amount of failed campaigns. There were very few canceled campaigns. 

## Analysis of Outcomes Based on Goals

###### Next, I analyzed the percentage of successful, failed, and canceled plays based on the funding goal amount. I organized the data into a new sheet, with respective data columns listed: Goal, Number Successful, Number Failed, Number Canceled, Total Projects, Percentage Successful, Percentage Failed, Percentage Canceled.

###### I then created rows that grouped the projects based on their goal amount, by dollar-amount ranges, as listed below:

- Less than 1000
- 1000 to 4999
- 5000 to 9999
- 10000 to 14999
- 15000 to 19999
- 20000 to 24999
- 25000 to 29999
- 30000 to 34999
- 35000 to 39999
- 40000 to 44999
- 45000 to 49999
- 50000 or More

###### I used the "COUNTIFS()" function to populate the Number Successful, Number Failed, and Number Canceled columns.

###### I used the "SUM()" function to populate the Total Projects column with the number of successful, failed, and canceled projects for each row. 

###### Finally, I calculated the percentage of successful, failed, and canceled projects for each row using the "ROUND()" function, and added the "IFERROR" function to change any errors to 0.

###### In order to visually represent this data, I created a line chart to visualize the relationship between the goal-amount ranges on the x-axis and the percentage of successful, failed, or canceled projects on the y-axis.

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/103145291/174224099-5565a408-f3cb-4493-b4b1-33c83aaa8955.png)

###### According to this graph, the rate of successful projects is indirectly related to the funding goal. However, some projects were successfully launched, even though they had a higher funding goal. The goals of these projects were between $35,000 and $44,999. 

## Challenges and Difficulties Encountered

###### Throughout this challenge, I struggled to find a reasoning as to why some of the projects from this campaign were successfully launched, even though their funding goals amounts were signiciantly high. This fluxuation did not match the overall relationship between the two variables: successful projects and funding goal.

## Results

###### Based on the data from the Outcomes Based on Launch Date Analysis, May would be the best month to launch, as it had the most successful kickstarter campaigns. However, there is also evidence to suggest that May, along with June, July, August, and October all had relatively similar numbers of failed campaigns launched. We can conclude that projects launched in May had both high rates of successs and failure; however, none were canceled.

###### The Alanysis of the outcomes based on Goals concludes that the rate of successful projects is indirectly related to the funding goal. However, there were a few projects that did successfully launch, even though their funding goals were on the higher range of $35,000 to $49,999. 

###### One limitaation of this data set is that it would have been beneficial to see the amount of funding used for marketing campaigns, as this can impact the spread knowledge of the project, prior to and during its launch. In the future, I would recommend finding data on the amount of marketing and forms of marketing done on each campaign and analyze it's relationship with the number of successful, failed, and canceled projects. 
