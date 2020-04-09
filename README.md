# ProsperLoan Data
### This project is part of Udacity Data Nanodegree program



### Dataset
The Dataset contains 113,917 loans, each loan has information on each borrower's annual percentage rate (APR), 
status, borrowed amount, debt, etc. Variables with missing values were dropped to make the Dataset more accurate. 
Outliers were also removed to provide more reliable Data. 
This investigation will be analyzing factors that could influence borrower's APR and what loans were taken by what type of borrowers.

#### library
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sb
import numpy as np
%matplotlib inline


## Questions

### I)Univariate Exploration
In this section, investigate distributions of individual variables. 
If you see unusual points or outliers, take a deeper look to clean things up and prepare yourself to look at relationships 
between variables.
**1)What factors affect a loan’s outcome status?**
-Choose 4 significant variables of income to plot which is Current , Completed,Chargedoff,Defaulted to plot bivate charts

### II)Bivariate Exploration
In this section, investigate relationships between pairs of variables in your data. Make sure the variables 
that you cover here have been introduced in some fashion in the previous section (univariate exploration).
**2)Are there differences between loans depending on how large the original loan amount was?**

-Completed loan has the most investor and ouliers , while people who are in debt have the lowest invest,
-Most of people in debt and people who past the dueday pay more often than others
-the other variables have realtive same mean of investors
-People who have high income range would around '25k- 49k' dollar rank the 1st in complete and charged off the debt, 
most of current loan is owned by the middle income '50k - 79k' dollar and default group most of them doesn't show income

**3)What affects the borrower’s APR or interest rate?**
APR la interestrate + origination fee adn docuemtnation fee, provide yearly rate
people  are curently in debt have really huge amount of oringial Loan amount
Charged off customers adn pastdue customers have the highest BorrowerAPR rate
III)Multivariate Exploration
-There is as strong positve relationship amoung `BorrowerARP`: with `EstimateEffectiveYield`,`LenderYield,EstimateLoss`,
`EstimateReturn`,`ProsperRating(Alpha)`

### License
MIT
