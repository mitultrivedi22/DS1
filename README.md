About Dataset
There are 29 variables of different natures with 1,048,575 rows. Data is maintained by data.gov Data.gov is the United States government's open data website. It provides access to datasets published by agencies across the federal government. Data.gov is intended to provide access to government open data to the public, achieve agency missions, drive innovation, fuel economic activity, and uphold the ideals of an open and transparent government.

Data Dictionary
CRASH DATE : Date reporting Crash
CRASH TIME : Date reporting Crash Time
BOROUGH : Near by Location
ZIP CODE : Zip Code of Crash Site
LATITUDE : Latitude of Crash Site
LONGITUDE : Longitude of Crash Site
LOCATION : Crash Site Location
ON STREET NAME : Street Name
CROSS STREET NAME : Cross Street Name
OFF STREET NAME : Off Street Name
NUMBER OF PERSONS INJURED : Person Injured
NUMBER OF PERSONS KILLED : Person Killed
NUMBER OF PEDESTRIANS INJURED : Pedestrians Injured
NUMBER OF PEDESTRIANS KILLED : Pedestrians Killed
NUMBER OF CYCLIST INJURED : Cyclist Injured
NUMBER OF CYCLIST KILLED : Cyclist Killed
NUMBER OF MOTORIST INJURED : Motorist Injured
NUMBER OF MOTORIST KILLED : Motorist Killed
CONTRIBUTING FACTOR VEHICLE 1 : Reasons for Collisions 1
CONTRIBUTING FACTOR VEHICLE 2 : Reasons for Collisions 2
CONTRIBUTING FACTOR VEHICLE 3 : Reasons for Collisions 3
CONTRIBUTING FACTOR VEHICLE 4 : Reasons for Collisions 4
CONTRIBUTING FACTOR VEHICLE 5 : Reasons for Collisions 5
COLLISION_ID : Collision Identification Number
VEHICLE TYPE CODE 1 : Vehicle Type 1
VEHICLE TYPE CODE 2 : Vehicle Type 2
VEHICLE TYPE CODE 3 : Vehicle Type 3
VEHICLE TYPE CODE 4 : Vehicle Type 4
VEHICLE TYPE CODE 5 : Vehicle Type 5
Problem Statement
There are over 2 million car accidents a year in the US according to the Centers for Disease Control and Prevention (CDC). Roughly, 42,915 people died in a fatal car crash in the US in 2021. Speeding accounts for more than 30 car accidents per day. Distracted Driving is a leading cause of car accidents. The number of drivers using cell phones behind the wheel has increased by 127% between 2012 and 2021. Auto accidents are a huge problem on US roads. A fatal car accident results in the death of 1 or more individuals. For American aged between 1 and 54, car accidents are a leading cause of death, according to the CDC. 1 in 10 fatal accidents are caused by distracted driving. Pedestrian and Cyclist deaths are on the rise. Calculations suggest that a fatal car accident occurs every 15 minutes in the US.

Project Scope
Data.gov started capturing motor vehicle collision data electronically after 2016. This data has many attributes like time and date of collisions, location, contributing factors, and types of vehicles involved in collisions. The Scope of the Project is to predict the likelihood of injury to a person if he/she is using motor vehicles considering the type of vehicle and contributing factors.

Further the project scope is decided as per email of 6th August 2023 to predict the number of motorist injured the requirement is set to treat this project as a classification problem (an not regression) and measure precision, recall, and F1 Score.

Method Used
Data Mining In Machine Learning. ML Models: Classification

Ensemble Random Forest Classifier

Rationale behind adopting Ensemble Random Forest Classifier
An Ensemble Random Forest Classifier is a machine learning algorithm that belongs to the category of ensemble methods. It's an extension of the basic decision tree algorithm and is designed to improve its predictive accuracy and control overfitting.

Here's how the Random Forest Classifier works:

Ensemble Method: An ensemble method combines the predictions of multiple individual models to improve overall performance. In the case of a Random Forest, the individual models are decision trees.

Randomness in Data: For each tree in the ensemble, the training data is randomly sampled with replacement. This process is known as "bootstrap aggregating" or "bagging." This means that each tree will see a slightly different subset of the training data, which introduces diversity and helps reduce overfitting.

Randomness in Features: Additionally, at each split point of a decision tree, only a random subset of features (variables) is considered for the split. This further enhances the diversity among the trees and helps in creating more robust models.

Voting or Averaging: To make predictions, the Random Forest Classifier combines the predictions of all the individual decision trees. In a classification task, this is typically done through majority voting, where the class that receives the most votes across all trees is selected as the final prediction. In a regression task, predictions are often averaged.

The key advantages of using a Random Forest Classifier include:

Reduced Overfitting: The combination of bootstrapping and random feature selection helps prevent overfitting. Individual trees may overfit, but by averaging their predictions, the overall model tends to generalize better.

High Accuracy: Random Forests tend to have high predictive accuracy due to the combination of multiple models and the reduction of overfitting.

Robustness: They are less sensitive to outliers and noisy data compared to a single decision tree.

Feature Importance: Random Forests can provide information about feature importance, which helps in understanding the contribution of different features to the model's predictions.

Model Evalution Metrics
Precision
Recall
F1
The Model is peforming weak despite the selection and application of robust classification model. It is evident that Regression Models are giving better and stable results compared to Classification Models. Precision, Recall and F1 is nothing but model evalution metrics just like Root Mean Squre Error. Selecting appropriate Machine Learning Algorithm is paramount important rather than choosing model evalution metrics. In the present case, Regression Models works best compared to Classification Models. However, this exercise is best example of knowledge sharing.

Observations
The most sensitive time during which accident might occured is 16:00 Hrs.
Top 3 vehicles invloved in accidents are sedan, utility vehicle and taxi.
Top 3 contributing factors for causing motor vehicle collisions are Driver Inattention, tailgating, and failure to yield right of way.
Recommendations
It appears that drivers are prone to make more mistake while driving from work location to home. Driving Speed limit should be reduced from 15:00 hrs to 18:00 Hrs.
The strategic traffic plans should be devised for vehicles like sedan, taxi and utility vehicles as they are highest contributors in motor vehicle collisions.
Unsafe Speed is the main cause for fatality hence it should be reviewed during specific time and location.
Next Step
To share this jupyter notebook with IT Team for deployment of Model.
