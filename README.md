# Supervised_Machine_Learning_Challenge
____________________________________________________

## Predicting Credit Risk
_____________________________________________________
![damir-spanic-vwaTtIhCjVg-unsplash (1)](https://user-images.githubusercontent.com/82990618/135730908-471a6b9c-9e12-4dc8-8699-0e6a51de18ed.jpg)


### Contributor: 

**Valense Acquah-Louis**

**For this homework, we use Supervised Machine Learning to predict if a loan from LendingClub will become high risk or not. **
LendingClub is a peer-to-peer lending services company that allows individual investors to partially fund personal loans as well as buy and sell notes backing the loans on a secondary market. LendingClub offers their previous data through an API.
Two machine learning models will be used to classify the risk level of given loans and to determine which works better or is more accurate. These models are, 
* Logistic Regression model and 
* Random Forest Classifier. 

**Source of data: **
* The Data as CSV were obtained from
    * LendingClub
* Selected Data
    * 2019loans.csv
   * 2020Q1loans.csv:

### The Analysis

**Preprocessing: Convert categorical data to numeric**

The entire years’ worth of data (2019) will be used to predict the credit risk of loans from the first quarter of the next year (2020).
A training set is created from the 2019 loans using pd.get_dummies() to convert the categorical data to numeric columns. Similarly, a testing set is created from the 2020 loans, also using pd.get_dummies(). 
Categories in the 2019 loans that do not exist in the 2020 loans testing set were filled by adding in the missing dummy variables to testing set. 

### Models

**Fit the models**

After the processing the data was fit to the Logistic Regression and Random Forest Classifier model to determine which was more accurate i.e., whether the Logistic Regression or the Random Forrest Classifier performed better. 
The models were scored

**Scale and Fit the Models**

Using StandardScaler, the training and testing sets were scaled. The scaled data were re-fitted to the LogisticRegression and RandomForestClassifier models and scored. 
Again, which model performed better was determined. 

### Prediction and Results

**Prediction**

*Unscaled Model*

Between the two forms of sklearn module (classification) I think the Random Forest Classifier will give a better result than the Logistic Regression, this is because in the Random Forrest Classifier the presence of the estimators which I look at as questions to help make the classification more precise helps make it more accurate. 

*Scaled Model*

Between the two forms of sklearn module (classification) I think the Random Forest Classifier will give a better result than the Logistic Regression irrespective of the data being scaled (i.e. making the data more uniformed due to difference in things like the units of, measure etc.), as stated above Random Forrest Classifier the presence of the estimators which I look at as questions to help make the classification more precise helps make it more accurate. 

**Results**

*Unscaled Model*

Between the two forms of sklearn module (classification) the Random Forest Classifier did perform better than the Logistic Regression as predicted, this is because in the Random Forrest Classifier 500 estimators were used and helped make the classification more precise/ accurate.  

*Scaled Model*

The results of the scaled data were not as predicted the testing score for the Logistic Regression was better than the Random Forrest Classifier, probably the Random Forrest Classifier was over fitted and the number of estimators my need to be changed
