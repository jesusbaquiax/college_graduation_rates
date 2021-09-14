![cover image](./Images/cover_image.jpg ){:height="300px" width="300px"}

# College & University Graduation Rates


## Table of Cotents

* [Overview] (#overview)
* [Business Understanding] (#business-understanding)
* [Data Understanding] (#data-understanding)
* [Data Preparation] (#data-preparation)
* [Model Training and Testing] (#model-training-and-testing)
* [Analysis and Conclusions] (#analysis-and-conclusions)
* [Next Steps] (#next-steps)
* [Project Structure] (#project-structure)


## Overview

One of the most important and stressful decisions a high school senior and their family have to make is deciding which college or university to attend. Colleges and Universities act as  gateways to potential financial success and opportunities. [Career earnings for a bachelor's degree graduate are more than twice as high as for someone with only a high school diploma.](https://www.brookings.edu/blog/up-front/2020/10/08/major-decisions-what-graduates-earn-over-their-lifetimes) While the financial prospects are a strong incentive for attending college or university, students are also taking out ever increasing loans to pay for college. [The average student loan debt for recent college graduates is more than $30,000 in 2019.](https://www.usnews.com/education/best-colleges/paying-for-college/articles/see-how-student-loan-borrowing-has-risen-in-10-years) Lastly, not all high school seniors have access to a college guidance counselor who can show them the application process and highlight institutions that offer scholarships, grants, or financial aids. [Only a third of country's public high schools have a counselor devoted to helping students get prepared for college, and the problem is even worse in high-poverty schools.](https://www.edweek.org/teaching-learning/college-advising-is-in-short-supply-in-u-s-high-schools-study-finds/2018/11) All of these are factors that students have take in account.

![money earned graph](./Images/money_earned_graph.png){:height="300px" width="300px"}

![student debt graph](./Images/student_debt_graph.png){:height="300px" width="300px"}


## Business Understanding

The American The College Counseling Association
this is how we will address the business problem....

## Data Understanding

The dataset was created by the U.S. Department of Education by matching information from the student financial aid system with federal tax returns. The dataset goes back all the way to 1998 and contains over 1,700 features. For the purpose of this project, the datatset was limited to currently operating institutions that offer predominantly associate's or bachelor's degrees from 2002 to 2012. The dataset is from [kaggle](https://www.kaggle.com/kaggle/college-scorecard).


## Data Preparation

There are over 1,700 features in the dataset and each can be broken up into school, admissions, academics, student, cost, aid, completion, repayment, and earning categories. 

Columns were dropped if they only contained NaN values, were outdated, or were a duplicate column.

Each feature category was approached separately in order to reduce running time and to make the preprocessing more manageable, but followed the general order listed below. 

For columns with NaN values, NaN values will be replaced with the median of the institution for that column. If the column still contains Nan values, the NaN values was replaced using a KNNimputer. The KNNimputer replaces missing values by imputing the mean value from nearest neighbors found in the set. Categorical columns were dummied out.

Then the correlation for the target variable was calculated for all the features in that category. The top five strongly correlated features for each category were placed in a list that would be used to create a new dataframe with all the strongly correlated features to be used for modelling.


## Model Training and Testing

After processing the data, the dataframe was still considerable large (~30,000, ~10,000)

baseline model score

first simple model

model 1

model 2

model 3


## Analysis and Conclusions

model X was out best model....

here are features that improved the models...

insert graphs


## Further Analysis & Implementation

Further analysis could be made by using more recent data from the U.S. college scorecard  after 2013 to see if the model could be improved on. With more data available, the model could also be narrowed to looking at institutions that predominantly grant bachelor's degrees. Finally, this project could be expanded to see how this model works with international institutions. 

This project could be used as the basis of new direct


## Project Structure


bash 
```

```