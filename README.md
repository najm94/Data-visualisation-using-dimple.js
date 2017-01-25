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

![v2_initial](https://cloud.githubusercontent.com/assets/23693349/22194857/c020f8ce-e16a-11e6-9b24-c3bd45037e77.PNG)

Finally,using "Age","Sex" and "Survived",I used a line plot to show the decreasing trend in survival rate with age.                 

![v3_initial](https://cloud.githubusercontent.com/assets/23693349/22194889/f5cf3544-e16a-11e6-8941-a8f9b96f1d90.PNG)

###Feedback       
####Feedback 1
I can clearly see the difference in survival rate for males and females in charts 1 and 2 but there is not title for any of the plots.I recommend using survival rate as a measure instead of survived in numbers.Also,I suggest that you group the ages into bins so that the overall trend in survival rate with age and also the plot will look more neat and less cluttered.Depending on what story you are trying to tell,i.e showing trends in survival rate with age or showing individual survival rate among age groups,choose a suitable plot.     

####Feedback 2
In the first and second visualisation,the story you are trying to communicate is survival rate by gender.So instead of using a simple bar chart,why don't you try a horizontal grouped stacked chart with suvival rate on x-axis and class on y-axis for visual 1 and port embarked on y axis for visual 2?It will better depict the differences among gender.Also,the third visualisation doesn't tell a clear story because the patterns are quite abrupt since you plotted survival for each age.Include titles for each visuals.        

####Feedback 3
Choice of plots is okay.But the problem with first and second visual is that the survival is in terms of numbers which is not a good measure here.I would suggest expressing it as a rate or percentageThe third visual looks a bit messy,so try binning the age groups for a smoother plot!Also,try other chart types for the third visual.Please add suitable x and y labels too.         

###Design changes after feedback   
Incorporating the suggestions from the feedback,I implemented the following changes:   
1.Added title for each visual    
2.Grouped the ages into bins     
3.Replaced the standard bar chart with horizontal grouped bar chart for visuals 1 and 2    
4.For visual 3,I replaced with vertical floating bars since I wanted the viewer to clearly see in which age group the survival rate was highest    
5.Added proper x and y labels   

####Visual 1 final version
![visual1_final](https://cloud.githubusercontent.com/assets/23693349/22195050/dd221d8a-e16b-11e6-8328-d7deda4ba1a8.PNG)   

####Visual 2 final version
![v2_final](https://cloud.githubusercontent.com/assets/23693349/22195211/cda51410-e16c-11e6-8dba-bacc5e59eca1.PNG)

####Visual 3 final version
![v1-final](https://cloud.githubusercontent.com/assets/23693349/22278473/c58615da-e2e9-11e6-9278-8c40c4ba0eda.PNG)


###Resources
1.https://github.com/allanbreyes/udacity-data-science/tree/master/p5   
2.http://dimplejs.org/index.html   

