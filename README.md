# Games Score
Are games getting worse?

One of my hobbies is playing online games with my friends, and as we were looking for a game to play, an argument arose about whether games are getting worse. As I'm entering the Data Analysis universe, I decided to look for a database and perform an analysis to answer the following question raised by my friends: "Are games getting worse?"
 
 Shall I start?
 
Well, at first I imported the necessary python language libraries and then loaded the database.Once loaded, I decided to check the data type in each column and if there was any null data that could mess up my analysis. After processing the data, I realized that the total number of games was equal to the total number of user and critic ratings per year, since for each game there was a user and critic rating. So when doing the "Year by Total Number of Games" graph I would be looking at two other similar graphs ("Year by Total User Ratings" and "Year by Total Critics Ratings").
 
 <div align="center">
 <img src="https://user-images.githubusercontent.com/106841477/172177663-695c3ecf-00ab-4742-ad39-2a5a46875be4.png"/>
 </div>
  
Based on the analysis of the "Year by Total Number of Games" graph, I decided to consider in the forward analysis only the years that had more than 100 reviews, both from users and critics, thus, from 2011-2018. 

<div align="center">
<img src="https://user-images.githubusercontent.com/106841477/172183925-15bec4c1-698d-4128-9b29-40550a8ea364.png"/>
</div>

However, there was a doubt on how to analyze: whether by the average or median of user and critic ratings. To check which one would be better, I made the boxplot of the user reviews and I noticed that in the period that it would be analyzed (2011-2018) there were many outliers, and the outliers significantly affect the average.

<div align="center">
<img src="https://user-images.githubusercontent.com/106841477/172184064-04c49a0b-4c7c-498e-8ba1-3901511a748a.png"/>
</div>

Therefore, using the median is a better choice in this case.

<div align="center">
<img src="https://user-images.githubusercontent.com/106841477/172184246-92b0eedd-d76d-4a31-941b-70aa4cad463c.png"/>
</div>
<div align="center">
<img src="https://user-images.githubusercontent.com/106841477/172184276-e4a4e43f-65ac-45a1-a580-6e44b8e44b68.png"/>
</div>

Answering the question "Are games getting worse?" The answer is perhaps no, because during the analyzed period (2011-2018) the scores remained consistent. However, there are flaws in the data that need to be taken into account, they are:
- The database is very small compared to the amount of existing games;
- There is a lot of user and critic ratings missing for many games;
- Many of the reviews from users and critics came from the same review site, so it may be biased.

For a business related analysis, it is best to look for another database or collect more data, but to answer my friends, it might be enough to end the discussion. The code used is available along with this repository.
