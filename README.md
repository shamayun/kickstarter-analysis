# An Analysis of Kickstarter Campaigns
## Overview of Project
Purpose of these analysis were to assist Louise to assess feasibility of her play, *Fever*, utilizing crowdfunding. This is her first crowdfunding project and she is hesitant as her budget already exceeded 10K. I would organize, analyze available previous data-set to assist her deciding factors such as timing, success of goal ranges so that Louise can kick start her fundraising on solid groud. Also, I would present the visuals of summarized data which would help Louise understand the previous trends quickly and repeat the success at ease.
## Analysis and Challenges
### Analysis of Outcomes Based on Launch Date & Challenges Encountered
My analysis started with finding a suitable time frame to launch theatre related fundraiser from the data set. This would help Louise to find the perfect time to launch her own theatre related fundraiser. All the related time data were available, yet in a different format that I needed to re-organize and present utilizing Excel's formulas. Launch date format was in Unix timestamps, theater information was jumbled up within subcategory data. I needed to convert dates to Excel standard form. I am aware that Unix timestamps starts from Jan 1, 1970 + seconds. I needed to use a formula to convert seconds to day, then added to Jan 01, 1970 to obtain the date. Once dates were converted to standard form, I was able to extract information for year using **YEAR** function. 

Theater related information was mixed with sub category data. Fortunately, parent category was separated with “/”. I was able to use “/” as a separator to use a formula(**FIND and LEFT**) to obtain parent category only. Now that the data are formatted, I am going to use a pivot table to summarize data by date and number of theater events by outcomes excluding live ones. The pivot table data shows previous trends by date, and success, failure, cancelled rate of the events.
### Analysis of Outcomes Based on Goals & Challenges Encountered
Now that Louise knows the suitable time to launch the fundraiser, I can help her finding a fundraising goal which would assist her visualizing the range(s) that are most successful. Louis is even keen on digging on sub-category of theater to know information relevant to *plays* only. 

I encountered similar challenge to get sub-category from mixed up data. Needed to utilized the separator “/” again. Using Excel formula(**FIND, RIGHT, and LEN**) in 2 steps I was able to segregate sub-category of theater-play. To identify successful project range, I categorized fundraising goal data into 12 categories, 9 of them in 5K intervals, 1 in less that 1K and 1 in more that 50K. Once categorized; utilized goal, outcomes, subcategory to filter data by respective ranges showing number of success, failure, and cancelled events. Summarized percentage of success, failure, and cancelled goals by ranges will help Louise to confidently launch her fundraising event according to her budget
## Results
Analyzing the data followings are the two conclusions about the Outcomes based on Launch Date:
1. Highest number of theaters took place in April-July(Summer), success rate is highest during those months
2. Overall success rate for theatre is 61%, best time to launch is Feb-July, Jan, Aug & Oct has success slightly below than average. December is the worst time to launch with highest failure and cancellation rate.

My observations about the Outcomes based on Goals:
1. Most successful plays had goals between 1-20k. Failure rate is average 65% when goal is 20k plus
-No cancellation for theatre plays at any time.

Even though 35K-45K goal ranges have great success rate (67%), there’s too few observations to rely on this data set. Data obtained for these analysis are not as current, latest data set is up March 2017. The current trend may have changed since 2017. Also, data includes from places all over the world, Louise’s target market is USA. We should rember these limitations while analysing the data,

I presented only line graphs to present/analyze findings. There are a lot of other possible options to consider including Bar graph, Histogram, Box and Whiskers are to name a few.

My recommendation to Louise will be to launch the fundraiser between February to July with a target of 10K-15K where the success rate is 2nd highest based on the number of observations. Even though the highest success rate is in the 35K-45K, number of obervations are few, and are outliers according to Box & Whiskers chart.

