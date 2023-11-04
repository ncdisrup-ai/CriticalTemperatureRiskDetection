# Critical temperature risk detection 
Detect risk of critical temperature in materials, through supervised machine learning

## 🤔 What is this?
**Description:**  How to detect risk of critical temperature in materials?.
Detect risk of critical temperature in materials, through supervised machine learning, testing 6 classification models and 6 regression models (w/CV) and their hyperparameters

Classification model  
- RandomForest              
- GradientBoosting                                    
- DecisionTree                                        
- LogisticRegression                                  
- SVC
- GaussianNB

Regression model  
- RandomForest_Regr
- LinearModel_Trees
- DecisionTree_Regr
- GradBoosted_Regr_Trees
- SVC
- Linear_Regr_Tree 

It involves Data Understanding, research and design of Artificial Intelligence supervised learning algorithms for **regression** and **classification** problems (we have two targets).

A typical data science project has several phases (Cross-Industry Standard Process for Data Mining (CRISP-DM)). Phases adapted to this project
1) Business Understanding: Understand the business problem and define the objectives of the project.

2) Data Understanding: Understand the data and its structure. We look at the data types, missing values, and other characteristics of the data. Discover and visualize the data to gain insights.
- Load Data
- PCA for reducing features (Need for?)
- Exploratory Data Analysis (EDA): Data Analysis Process with estatistical analysis and data visualization for knowing data and obtain findings
a) Data Exploration: Examining summary statistics, visualizing data distributions, and identifying patterns or relationships.
b) Data Visualization: Presenting insights through plots, charts, and graphs to communicate findings effectively

3) Data Preparation: Prepare the data for modeling by cleaning it up and transforming it into a format that can be used by machine learning algorithms.  
- Data Cleaning: Handling missing values and categorical values, removing outliers and duplicates, and ensuring data quality.
- Data Transforming
- Feature Engineering: Transforming variables, creating new features, or selecting relevant variables for analysis.
-- Feature selection: selecting the most useful features to train on among existing features. 
-- Feature extraction: combining existing features to produce a more useful one (e.g. handling missing data, encoding variables, dealing with categorical variables, dimensionality reduction algorithms ...). 
-- Creating new features by gathering new data.
- PCA for reducing features (or in the begining after loading data) (need for?)
- Data Visualization after Data Preparation: Presenting insights through plots, charts, and graphs to communicate findings effectively

4) Modeling / Select and Train Models: We create a model that can be used to make predictions or classify new data. 
- Retrieve Class (y) from the dataset (X)
- Split Data
- Normal Test
- OverSampling (SMOTE) and undersampling (need for?)
- Calculate the weights for each sample based on the feature (transaction amount) and class weight (need for?)
- Intermediate Results (need for?)
- Train model (w/cross-validate) (based on OverSampling (SMOTE) and undersampling) (need for?)

5) Evaluation: We evaluate the model’s performance and determine whether it meets the business objectives.
- Evaluation using cross-validate
- Fine-tune Models  
- Model Evaluation on Test Set

6) Deployment Deploy the model into production and monitor its performance over time.


## 📚 Data

Data with the projects (to train the model and to apply the model) are in data dir.
 
Consider the data `HA1-DatasetScaled.tsv` and obtain a model to detect risk of critical temperature in materials.

Objective 1
- Produce the best regression model for critical_temp (Dependent Variable)

Objective 2
- Produce the best binary classification model assuming as positive all instances with values of critical_temp >= 80.0 and as negatives all remaining cases


##  🚀 Quick Install


jupiter notebook (.ipynb) file in model dir


## 📖 Documentation

Please see the description in .ipynb about this project.


##  🚀 Results 
