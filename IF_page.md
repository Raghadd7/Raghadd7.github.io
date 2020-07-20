## Identifying Factors Involved in Road Accident Using Data Mining Techniques
#### A team project conducted to identify the factors that are involved in road accidents in the United Kingdom 

**Abstract** car accidents are considered a serious issue in every country, especially when the cars are usually considered the main transportation method. 
It costs the lives of the drivers, passengers and pedestrians. In this paper, a study was conducted to investigate which factors are the main cause of 
car accidents severity using the UK car accidents’ dataset. Feature selection process was applied using the random forest to get the features’ importance, 
along with the association rules. The used methods in the study were the decision tree and the random forest as the learning models to predict the accident 
severity. Furthermore, to enhance the results these learning models were applied in collaboration with AdaBoost to increase the metrics’ results, where the 
best model gained an accuracy of 84.95%.These models were applied after balancing the dataset to remove the unbiased case in the targeted feature.



**Introduction** Road accidents are a global serious threat, as it results in severe injuries, disabilities and it even costs peoples their lives. According to World Health
Organization (WHO) global status report on road safety in 2018 reported that road accidents causes more than 1.35 million deaths each year and up to 50 
million injuries. Therefore, mitigating these accidents is an important area to look into. 

The main purpose of this study is to address the severity of the accidents, and what is the cause of such accidents to be severe. In general, 
the severity of accidents can be categorized into accidents with slight, serious and fatal damage to the people involved. 
For that, three different data analysis types should take place in this study. The first being the descriptive analysis to describe the current situation, 
and then the diagnostic analysis to find the reason of such situation to happen.

In order to provide effective solution to the addressed problem, there were two main issues needed to be confronted: unbalanced data 
classes for the independent variable, and feature selection due to the huge number of features in the dataset, and to select which of the features are 
the main factors to affect the accidents’ severity.



**Data description**

In this study the UK accidents dataset afforded by Kaggle is used. it provides detailed traffic data about road accident from 2005 to 2014. 
This data is a 10 years historical data divided into three datasets: accident, vehicles and casualties’ datasets each of which are at the size of 1.6m, 
2,2m and 3m records respectively. The aim of this study is to investigate the most important factors that affects an accident severity using data mining 
and data analytics techniques. The objective of this workis to assess the performance of the learning models after balancing the data.

The accident’s dataset contains the general information of an accident such as: accident severity, weather, location, date, hour, day of the week, road type...etc.
Whereas, the Vehicle dataset describes the vehicle conditions which was involved in the accident like the vehicle type, model, engine size, driver sex, driver age,
car age...etc. The third dataset which is the casualty dataset has the information of the people involved in the accident such as the severity of the causality’s 
condition, their age, sex social class, casualty type, pedestrian or car passenger. The accidents and the causality datasets together will cover the aspects to be investigated in this study, where the vehicle dataset might be used in future work 
to uncover further factors.


In order to start the analysis and to deliver good results, it was essential to understand the data at the beginning. 
For this reason, an exploratory analysis was done which includes data assessing to find different issues in the data. 
The steps are divided as the following subsections:

**A. Exploratory Data Analysis (EDA)**

Data exploration is to identify the data’s proportions and the nature of the values each feature may hold. 
In this study, we are interested in finding the cause and which factors of the accidents and what causes the severity to vary from accidents to another.
Therefore, the vehicle dataset was considered as a source out of the context of this study and would not be considered in this scope. 
After that, the accidents and casualty datasets are merged by the accident index feature which works as a unique identification to each accident. 
The merge of these two datasets have resulted in gaining 46 attributes and 2216720 records as a final dataset.
The dataset was explored and assessed by using the library pandas_profiling which in return performs basic analysis to give more valuable information
about the data. The following figure illustrates a basic overview on the dataset, as well as the missing values and high correlated variables. 
This profiling works as a data assessing report which highlights the major issues to be found within the data, which leads to which cleaning techniques 
to be followed.

<img src="images/profiling.png?raw=true"/>















**Conclusion**

After applying the learning models on the balanced dataset, it was apparent that the provided metrics results had consistency which shows 
the reliability of the model to give accurate results for this study. In addition to that, the feature selection method had given the top 
factors that affect the severity of the accidents. These features were tested using the RF and DT learning models where the high and stable 
results have concluded the effectiveness of balancing the data and the accuracy of the selected features by the algorithm.

