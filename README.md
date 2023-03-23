# Heart Disease Prediction Model
Model that will predict whether or not a patient has heart disease.

For this purpose, we have the following data set.
![Dataset](./images/dataset.jpg).

Steps for training the model.
### 1. First we import the dataset with pandas.
![Import Data Set with pandas](./images/import_dataset.jpg)
### 2.  Data preparation.
Data cleaning, we replace categorical data with mode, numerical data with mean. Then data splitting for training and testing.

Delete the column 'HR' because have 80% the data is null.
![delete_hr](./images/delete_hr_80_porcent_null.jpg)

Replacing the null data with the most frequent value to the categorical variables.
![replacing_data_categorical](./images/reemplace_data_category.jpg)

Replacing the null data with the average value to the numerical variables.
![data_replacing](./images/remplacing_data_mean.jpg)

As can be seen in the following output we no longer have null data.
![no_data_null](./images/no_data_null.jpg)

We separate the variables into outputs (the DIAG variable), and inputs (the rest of the variables).
![separate_data_diag](./images/data_uotput_DIAG.jpg)

We standardized the numerical input variables, and coded the categorical input variables. We code the categorical input variables, Standardize the numerical input variables.
![data_standrdized](./images/no_data_null.jpg)

#### We split the data for training and testing.
![data_split](./images/split_data_train_test.jpg)

### 3. Train the Logistic regression model
Trained models take unseen data and give an estimate if the patient does or does not have heart disease.
![train_model](./images/train_model_logistic_regression.jpg)

Confusion_matrix
![confusion_matrix](./images/confusion_matrix.jpg)

With an accuracy of 0.84878048487804878 training and with an accuracy of 0.8314606741573034 testing with unknown data.

### 4. Evaluate the model.
Check the accuracy of the predictions with the unknown data
![evaluation_model](./images/evaluation_model.jpg)
