# uber-hypothesis-testing

## Purpose
Design and create the hypothesis testing, to analyze the SFO and LAX data sets, determine if either marketing campaign was successful in raising the average miles driven per Uber driver.

## Dataset
From Uber's dataset including both SFO and LAX marketing campaign information. 

Feature Definitions
- Date: the date that the observation was recorded.
- Avg. Daily Miles Driven Per Hour: the avarage of daily miles driven per hour.
- Marketing_Campaign: a binary field that is set to either 1 for when the marketing campaigns were active or 0 for when the marketing campaigns were deactivated.

## Test Setup
#### The Null Hypothesis (H0): 

The average daily miles driven per hour when the marketing campaign was in service is the same as the average daily miles driven per hour when the marketing campaign was not in action.

#### The Alternate Hypothesis (H1): 

The average daily miles driven per hour when the marketing campaign was in service is greater than the average daily miles driven per hour when the marketing campaign was not in action.

#### The p-value will be set to .05


## Conclusion

#### SFO Campaign
![image](https://github.com/miayuxin/uber-hypothesis-testing/blob/master/image/SFO.png)

![image](https://github.com/miayuxin/uber-hypothesis-testing/blob/master/image/SFO%20result.png)

The result is p = 0.000. If the p-value is less than 0.05, we reject the null hypothesis. Meaning that marketing campaign does not help in raising the average miles driven per Uber driver.  

However, I found that even the null hypothesis was rejected, alternative hypothesis was not supported. On the contrary, the distribution plot shows that the average daily miles driven per hour when the marketing campaign was in service is less than the average daily miles driven per hour when the marketing campaign was not in action. How does this happened? I assume that is because we only consider the relationship between average mile and marketing campaign. There are other features affecting the average miles driven per Uber driver. For future work, we should consider other factors. (refer below follow-up)


#### LAX Campaign 

![image](https://github.com/miayuxin/uber-hypothesis-testing/blob/master/image/LAX.png)

![image](https://github.com/miayuxin/uber-hypothesis-testing/blob/master/image/LAX%20result.png)

The result is p = 0.345. If the p-value is greater than 0.05, we failed to reject the null hypothesis. The distribution plot shows that marketing campaign was successful in raising the average miles driven per Uber driver.


#### Follow-up - What factors may affect the validity of this study?

- Weather: sunny day or rainy day might bringing a variation in the average miles driven per Uber driver. On a rainy day, probably more people taking Uber or not taking Uber, that affect the average mile driven by per driver.
- Time: weekday, weekend, and holiday season may impact. For example, the average miles driven per Uber driver may increase, during weekend or holiday season, since more people or tourists ride Uber.
- Economic: during economic recession, the number of rides might decreased, which reducing the average miles driven per Uber driver.
- Competitors: if the competitors such as Lyft or Carpool services appear and offer the coupons or lower pricing may impact the average miles driven per Uber driver.