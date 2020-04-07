# DATA1030-HR-Data-Analysis
Course DAT-1030 Assignment #5

The problem that being analyzed is how to try and predict the attrition of valuable employees. 
The aim was to try and uncover the factors that lead to employee attrition and explore important questions such as ‘show me a breakdown of distance from home by job role and attrition’ or ‘compare average monthly income by education and attrition’. This is a fictional data set created by IBM data scientists. It is apart of the IBM HR Analytics Employee Attrition & Performance initiative.


Insights found
---
I was discovered that presons earning less than $1000 in sales were twice as likely to leave than to stay.
It was also seen that 20% of persons earning $20000 a month was just as likely to leave.
It was clear however that the majority of staff earning $4000 were like to stay.
The rate of attrition fell significantly when the monthsly sales earning increased above $4000 a month.

There are insights from Lucas Fischer that were also informative:
"Employee churn can be a sensitive topic in certain cases (for example, giving a raise to an employee based on the prediction a ML model made, can be misinterpreted by other employees, or even you can be giving a raise to the wrong employee).

Since there is no time-series in this dataset, all classification tasks, in the various and cool notebooks this dataset has, have been to train a machine learning model on a portion of the employees and test it on the remaining, unseen, portion of employees. What this tells you is that if the conclusion and assumptions you made generalize to unseen employees. Given this holds true you can make conclusions about the entire population because you know they will be right in general.

However, say X number of months pass and you want to re-predict who is going to churn or not. Your model won't be able to do this because this is not what it was trained for. Your model was trained to distinguish between the two populations, churners and non churners, given they are all in the same time-step. It was not trained to know if an employee will leave X months in the future, and it was not trained to generalize to other time-steps in the future.

So be careful if you wantted to apply a model like this in your company. If you want to predict for the same employees but in different times in the future, then the models you have in these notebooks woun't do. There is still interest however in being able to distinguish the two populations as it gives you insight as to what makes them different!"


This directory structure of the Project is:
1. Data :- folder containing raw data accessed to do the analysis on HR Sales
2. Munge :- Folder contains scripts used to transform the data for upload to Hive repository
3. Src :- Folder contains scripts with aggregations used to prepare data for analysis.
4. Reports :- Folder contains spreadsheet with dashboard displaying the visualizations of the data and the insights found

