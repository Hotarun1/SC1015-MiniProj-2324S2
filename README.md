# SC1015: DSAI Mini Project - Multiple Disease Detection


### Description:
This repository contains all Jupyter Notebook (.ipynb) files, datasets, videos, and source materials/references used (if any) that have been created/used as part of SC1015 DSAI Mini Project.  
This README will highlight the main pointers and actions taken in the project. For more details, refer to the .ipynb files in this repo.

### 1. Problem Formulation:
Dataset Chosen: [Mutliple Disease Prediction](https://www.kaggle.com/datasets/ehababoelnaga/multiple-disease-prediction)

**Problem Statement:** How might we detect various types of diseases using blood work results?


Blood work is one of the most common tests done in the medical field. Could we develop a predictive model that can identify the likelihood of various diseases based on the provided blook work results provided by the lab?

A successful high-confidence model may be able to significantly impact patient care by allowing precise and early diagnostics, improving treatment outcomes, and optimizing resource allocation.

In the likely chance that the model may not have a high confidence in predicting the diseases. It could serve as a flag of sorts; placing more emphasis on certain few patients that may encounter such.

### 2. Data Preparation
The dataset chosen was already pre-cleaned and managed well. There was little to no preparation and cleaning needed to analyze our data better.


### 3. Exploratory Data Analysis
Various visualisation methods was used, namely histogram, bar chart (count of diseases) and violin plot. They were mainly used to observe trends and distributions of each of the variable.
Logistic regression was then applied to find out the coefficients of each variable, how likely/unlikely would the presence or absence of the variable affect the presence of each disease.
The results were that **Diastolic Blood Pressure**, **AST (Aspartate Aminotransferase)** and **BMI (Body Mass Index)** does not impact the likelihood/unlikelihood of diseases as much as the other variables due to the low coefficent value.

As a result, we will be leaving them out in order to cut down the number of variable that the model will be trained on.

### 4. Model Used
The dataset used mainly consists of classification variable therefore, we will be using Gradient Boosting Classifier, Decision Trees, Random Forest, and Support Vector Machines models.

After evaluating the models used above, we continued by applying **ensemble techniques** namely, stacking to help improve the final prediction, utilising the strengths of **Random Forest**, **Gradient Boosting** and **Support Vector Machine**.

### 5. Conclusion
Although the accuracy of the model may not be high overall, with the usage of the stacked model, the models could be used as a sidekick for medical professionals to highlight possible diseases (**Diabetes** (Moderate/High Confidence), **Anemia/Thalasse/Thoromboc** (Low/Moderate Confidence)).

The project was overall a success in aiding us apply various machine learning models and data science technique to attempt to solve real world problems.
Although there was no concrete solution found in the short term, it helped us apply the knowledge gained in SC1015. In the future as technology advances, there could be an algorithm that would be able to predict with full confidence.

### 6. Contributors
@Hotarun1 - Leo  
@JerwinLee3690 - Jerwin  
@Sandwhich253989 - Avanesh  

### References
Advanced Ensemble Techniques - [https://towardsdatascience.com/advanced-ensemble-learning-techniques-bf755e38cbfb]
