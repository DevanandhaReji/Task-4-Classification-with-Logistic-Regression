# Task-4-Classification-with-Logistic-Regression
Task 4: Classification with Logistic Regression
1. Importing Libraries
The following libraries were imported:

pandas and numpy for handling and processing data

matplotlib for plotting graphs like the ROC curve

sklearn modules for preprocessing, model building, and evaluation

2. Loading the Dataset
Since the dataset was in Excel format, I used pandas.read_excel() to load the data into a DataFrame for further analysis.

3. Data Cleaning and Preprocessing
Unnecessary columns such as id and any unnamed columns were dropped.

The target column diagnosis was converted from categorical (M, B) to numeric (1, 0) using label encoding.

The features (X) and labels (y) were separated.

4. Train-Test Split
The dataset was split into training and testing sets using an 80:20 ratio to ensure that the model could be evaluated on unseen data.

5. Feature Scaling
The features were standardized using StandardScaler to ensure that all input features have zero mean and unit variance. This improves the performance of the logistic regression model.

6. Training the Logistic Regression Model
A Logistic Regression model was trained on the scaled training data using LogisticRegression() from the sklearn.linear_model module.

7. Making Predictions
After training, predictions were made on the test data using the trained model.

8. Evaluating the Model
The model's performance was evaluated using the following metrics:

Confusion Matrix: Shows correct and incorrect predictions in a matrix form.

Classification Report: Provides precision, recall, F1-score, and support.

ROC Curve and AUC Score: Shows the true positive rate vs false positive rate, and the AUC (Area Under the Curve) value indicates the overall classification performance.

9. Saving the Processed Data
The processed and scaled datasets (both training and testing) were saved as:

processed_train_data.csv

processed_test_data.csv

These files include the scaled features along with the diagnosis label column.

Result
The model achieved high accuracy and a strong AUC score, showing that Logistic Regression is effective for binary classification on this dataset.
