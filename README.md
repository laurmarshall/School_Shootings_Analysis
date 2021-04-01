# The American Way?
![](https://github.com/laurmarshall/School_Shootings_Analysis/blob/main/images/school-shooting-header.jpeg)
## A Look at School Shootings and Gun Laws in the United States
### Lauren Marshall, Data Scientist
[LinkedIn](https://www.linkedin.com/in/lauren-marshall-7603491b5/)|[GitHub](https://github.com/laurmarshall)|[Slides](https://github.com/laurmarshall/Burnout-In-Tech/blob/main/Burnout%20in%20the%20Tech%20Industry.pdf)
## Background and Motivation
Since 2009, the [United States](https://www.cnn.com/2018/05/21/us/school-shooting-us-versus-world-trnd/index.html) has had over 57 times as many school shootings as Canada, France, Germany, Japan, Italy, and the UK combined. This is not a statistic you want your country to be leading in.
[Trends](https://www.cnn.com/interactive/2019/07/us/ten-years-of-school-shootings-trnd/) show school shootings are on the rise. They are more likely to happen in urban areas and the risk of casualities increases if the student body is primarily white.


As a former educator, for almost a decade I personally participated in countless active shooter/lockout drills. I have had many conversations/answers student questions about what would happen if a stranger where to come to our classroom with a gun.

## The Data
The data consists of three different datasets from [Kaggle](https://www.kaggle.com/):

- [School Shootings US 1990-Present](https://www.kaggle.com/ecodan/school-shootings-us-1990present): This dataset includes two dataframes. It was last updated in October of 2020.
  - One with the date, location (City and State), are type (rural, suburban, and urban), school type (nursey, elementary, middle school, high school, and college), fatalities, wounded, the source (Wikipedia or ), and description (for the Wikipedia sources). There were some null values and duplicates in this dataframe that had to be cleaned. This was the main source for the analysis.
  - The second dataframe included census information for each school type.

- [Firearms Provisions In US States](https://www.kaggle.com/jboysen/state-firearms):This dataset includes two dataframes.
  -One with the listing of all fifty states for each year from 1991 - 2017, which gun laws each state followed, and a total count of guns laws for the state.
  -The second dataframe include a description of each column (each gun law) in the first dataframe. This broke down the implication for the dealer, the buyer, specifics for handguns, waiting periods, ammunition, etc.

- [Gun Ownership By State](https://www.kaggle.com/solorzano/gun-ownership-by-state): This dataset from 2018 included one dataframe with all fifty states and the District of Columbia. It included the number of guns per capita and the number of registered guns per state.


## Exploratory Data Analysis
![US School Shootings by City](https://github.com/laurmarshall/School_Shootings_Analysis/blob/main/images/US%20School%20Shootings%20by%20City.png)


![US School Shootings: Fatalities and Number of Events](https://github.com/laurmarshall/School_Shootings_Analysis/blob/main/images/US%20School%20Shootings:%20Fatalities%20and%20Number%20of%20Events.png)
### Machine Learning Techniques
Gradient Boosting returned the highest percentage with a R2 score of 71%.

### Graphs
![Time Series Prediction on Number of School Shootings](https://github.com/laurmarshall/School_Shootings_Analysis/blob/main/images/Time%20Series%20Prediction%20on%20Number%20of%20School%20Shootings.png)

![Time Series Prediction on Gun Laws](https://github.com/laurmarshall/School_Shootings_Analysis/blob/main/images/Time%20Series%20Prediction%20on%20Gun%20Laws.png)

### Natural Language Processing

## Conclusion
The issue at hand is simple, but the factors are complex. It is simple becuase school shootings are on the rise in the US and so student and teacher safety is at risk. No one wants innocent children to die. It's complex because how do you can you predict and plan to improve somethings when likely, one of main factors is human behavior?

The most common shooting location was high schools, accounting for 59% of the data. Reading through the descriptions time and again the shooter is described as a teenager themselves. One of the disputes was over $40 dollars. A 14-year-old killed another 14-year-old over $40. The [prefrontal cortex](https://www.nimh.nih.gov/health/publications/the-teen-brain-7-things-to-know/index.shtml), the part of the brain that regulates decision making and manages impulses is fully formed until aroudn age 25. As a result, the teenage brain too often relies on the amygdala, or emotional center, of the brain to makes decisions. This is an important consideration in addressing this epidemic.

## Questions and Future Studies
1. What would updated data present? What impact has the pandemic had? What further impact will it have? With a significant amount of school being remote during the spring of 2020 and for much of 2020-2021 school year school shootings have recently declined. But as we have seen in recent news, within a week there was a mass shooting in Atlanta, GA and then Boulder, CO. What does this mean for schools?

2. What is the global significance? Why is it that the US has such higher numbers for school shootings than many other countries? Does this connect to our [higher rates of prisons](https://www.prisonpolicy.org/global/)? What impact does culture in the US play?

3. What other factors are important to consider? Are there more shootings during certain times of year? Does the SES of the community impact the risk? One of the main arguements regarding gun laws is that guns don't kill people, people kill people. What role does mental health play? Connecting back to question 2, how significant is the American (white male) ego? The [mass shooter in Atlanta](https://www.nytimes.com/live/2021/03/17/us/shooting-atlanta-acworth) committed a hate crime based on his sex addiction. Instead of working on his addiction internally to seek help, he chose to outwardly eliminate "temptation" and kill other innocent people. Is the US more reactive than proactive in their efforts?

4. Finally, are there any common threads with mass shootings? A mass shooting is generally defined as an incident with 4 or more death from someone with a gun. When looking at school shootings are the any differences between those with 3 or less fatalities and those with 4 or more? Are there any unigue indicators for schools to be aware of? 
