# fifa21-project
***
For our first group project we were given the task of predicting a player's "Overall Rating" (OVA) by analising data. Our main tasks were cleaning and preparing the data, processing it, training and testing a Linear Regression model, and validating it. I worked with Lara and Diego in this task. 

## Decisions
As we were unfamiliar with the formula and could not find an exact one in our research and observation of the dataset, we intuited the potential of the scores of their attributes plus their best position scores. Our main decisions for this approach are:
    1. OVR = ATT + IR (Overal Rating equals attributes and international reputation).
    2. For those columns with "+", we're going to keep the second number. We believe the first number can be calculated from the columns of atributes, although we are unsure as to how.
    3. By initial sum through categories in the given resource page of player profiles, we now know some columns are the sum of other columns. We decided to keep the most of the information for the model to better understand the patterns.

## Conclusions
- We could see that these validation scores help us see that there is some dependancy on the stats, giving 1 or 2 numbers off in the mark of difference.
- To improve our model, we compared our initial with a reduced correlation (dropping any corr under 0.2) and one without this condition plus adding the wage, as we believe their salary could influence this value aside from the formula ones identified.
- We could see a slight improvement in the model with a +0.01 change in the R2 score, and one of -0.06 on the RSME score.
- We could see that these validation scores help us see that there is some dependancy on the stats, with some slight influence regarding wage.

***
#### Links to review terminology:
- Explanations of the acronyms and abbreviations can be found here (https://gaming.stackexchange.com/questions/167318/what-do-fifa-14-position-acronyms-mean) and here (https://fifauteam.com/fifa-ultimate-team-positions-and-tactics/)
- FIFA 19 player rating guide (https://fifauteam.com/player-ratings-guide-fifa-19/)
- FIFA overall rating explained (https://earlygame.com/fifa/fifa-ratings-explained-overall-rating)
- FIFA 21 all attributes divided (https://fifauteam.com/fifa-21-attributes-guide/)
