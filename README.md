# Data-visualisation-using-dimple.js
##Data visualisation of titanic data

The titanic dataset contains demographics and passenger information from a subset of the 2224 passengers and crew on board the Titanic.

###Summary
In creating my visualisations,I use the variables passenger class(Class),the port from which the passengers embarked(Embarked),gender('Sex') and age('Age') to study their influence on survival rate.The goal was to show that female passengers had higher rate of survival whether we look across passenger class,the port embarked or by age group.

1.The first visual shows the survival rates by passenger class by gender                                       
2.The second visual shows the survival rate by port embarked by gender                    
3.The third visual shows the variation in survival by age groups                 

###Design
####Exploratory analysis using python
I used Numpy and Pandas libraries in python to understand the variables involved and how it affects the survival.As a result of my investigatiom,I understood that females have higher chance of survival than males even when we look across different passenger classes,or the port embarked.Binning the ages into groups,I was able to detect difference in survival rates.                  
I am using dimple.js charting library in creating my visualisations.                             

####Initial choice of chart types

First I explored Passenger class('Class') and survival by gender('Sex').                  
Here both Class and Gender and categorical variables.So,to represent the number of survived people in each category, I used bar chart.
Visual encoding:the x-axis represents Class.Color is used to reprsent Sex.y-axis represents number of survived people.    

![v1_initial](https://cloud.githubusercontent.com/assets/23693349/22194779/6cdedcf8-e16a-11e6-8d6a-e53f84489e10.PNG)       

Next,I used 'Embarked' and "Survived" by "Sex"
Embarked is also a categorical variable.So ,here also I used a bar chart.
Visual encoding:x-axis represent port embarked,y-axis reprsents people who survived and color rpresents male or female.      

