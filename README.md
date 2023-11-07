# Bank-Customer-Churn-Prediction
## Task
Build a machine learning model to predict where a customer will contine with the bank or not(Churn).</br>
Tool Used: Python, Jupyter Notebook
## Dataset:
Dataset is taken from Kaggeles "Bank Turnover Dataset". Dataser contains 10000 different datas with 14 features.
- RowNumber : int type
- CustomerID: unique value of the customer
- Surname: Surname of customer, object type
- Credit Score: int type
- Geography: France, Spain and Germany
- Gender: Male, Female
- Tenure: No of Years
- Balance: Customer Account Balance
- Number of Products: How many accounts, bank account affiliated products the person has. Values are 1, 2,3 and 4
- HasCrCard: Does the customer have a credit card through the bank? 1 , 0
- IsActiveMember: 1, 0
- EstimatedSalary: Customer Salary, type float
- Exited: Did they leave the bank after all? Yes: 1, No: 0 </br></br>

Credit: Bank Turnover Dataset, TARUN SUNKARANENI, https://www.kaggle.com/datasets/barelydedicated/bank-customer-churn-modeling/data

## Step Followed:
### Load the necessary Libraries:
- numpy
- pandas
- matplotlib
- seaborn
- StandardScaler
- train_test_split
- Tensorflow
- keras
- confusion matrix
- classification report
- display from IPython
- SMOTE from imblearn.over_sampling
### Data Collection, Analysis and Processing:
- Load the data using pandas read_csv
- Remove the irrelavent coloumn
- Perform **Data Visualization**
  - Analyse Categorical Column
  - Analyse Numerical column
  - Compare all features with the target column
- **Data Processing**
  - Convert the Categorical text column to numerical column
  - Standardize the data using Standard Scaler library
### Model Building
- Split the data into feature and target
- Split the feature and target into Training and test sets
- Function to build a model
  - Build the Neural Network Model using keras
  - Compile the model
  - Get the Y_predict values
  - Train the model
  - Plot the loss and accuracy
  - Print classification report
- Plot the classification report
- Plot Confusion Matrix
- **Handling the Imbalanced Dataset**
  - Synthetic Minority Oversampling Technique(SMOTE): SMOTE first selects a minority class instance a at random and finds its k nearest minority class neighbors. The synthetic instance is then created by choosing one of the k nearest neighbors b at random and connecting a and b to form a line segment in the feature space. The synthetic instances are generated as a convex combination of the two chosen instances a and b.
  - Get the new set of X and Y sample using SMOTE, the sample contains equal number of both the classes
  - Perform the same train_test_Split and model building method
  - Plot the classification report and Confusion Matrix</br></br></br>

