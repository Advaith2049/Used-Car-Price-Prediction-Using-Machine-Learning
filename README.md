# Used-Car-Price-Prediction-Using-Machine-Learning

### **Used Car Price Prediction: An Overview**  

* Cleaned the dataset, removed outliers, and pre-processed the data in a format suitable to the objective 

* Performed extensive EDA or Exploratory Data Analysis to understand the relationships between the variables and data points 

* Fit the processed data into various models including Linear Regression, Random Forest, KNN, SVM, among several other algorithms, to make predictions and arrive at the best model through comparison 

* Charted a comparison table for the ease of determining the best model and accuracy


### **Codes and Resources Used**

* **Programming Language:** Python 3.11.1

* **Packages:** pandas, numpy, seaborn, matplotlib, scipy, sklearn, statsmodels, tensorflow

### **About the Dataset**

* The Car Price Prediction dataset has a total of 18 columns and 19237 rows.

* There are no null values across the data, and the data types range from 'object' type to 'integer' type.

* The target (or) dependent variable which needs to be predicted is the column 'Price' 


### **Data Cleaning**

After the data was loaded in with pandas, it was cleaned, and the following changes were made:

* Columns like ‘Prod. year’, ‘Engine volume’, ‘Gear box type’, among others were renamed to more simpler and suitable names

* Data columns were divided into numeric type and object type for the ease of working and conversion

* ‘ID’ column was dropped

* ‘km’ string was dropped from the ‘Mileage’ column and was converted into a float column

* ‘Engine_vol’ column was standardized by the creation of another column, ‘Engine_type’, which stored binary values of ‘Turbo’ or ‘Non-Turbo’

* Outliers were detected in the columns – Levy, Cylinders, Airbags, Engine_vol, Mileage, and Price, and subsequently removed


### **EDA (Exploratory Data Analysis)**

Some highlights of the EDA are as follows:

![alt text](https://raw.githubusercontent.com/Advaith2049/Used-Car-Price-Prediction-Using-Machine-Learning/main/images/CPP1.png "Logo Title Text 1")




### **Feature Selection and Pre-Processing**

* VIF or Variance Inflation Factor was utilised to select the features that would influence the target variable the most. 

* ‘Cylinders’, ‘Engine_vol’, and ‘Levy’ were dropped to ensure a better VIF score and less multicolinearity.  


### **Model Building**

The categorical variables were first transformed into dummy variables using ‘OneHotEncoder’ and ‘ColumnTransformer’. Then, the entire dataset was split into training and testing datasets of the ratio 80:20. Multiple models were applied and MAE or Mean Absolute Error was the metric used to evaluate these models. 

The applied models were:
* Linear Regression
* Boosting (Gradient, Ada Boost, XG Boost)
* Bagging
* Decision Tree Regressor
* Random Forest Regressor
* KNN
* SVM
* Neural Networks


### **Model Performance**

The Bagging Repressor outperformed all the models and the model comparison table is as follows:

