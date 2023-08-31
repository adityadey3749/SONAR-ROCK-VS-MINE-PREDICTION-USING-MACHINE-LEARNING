# SONAR-ROCK-VS-MINE-PREDICTION-USING-MACHINE-LEARNING

## Dataset link for this Project (SONAR ROCK VS MINE USING MACHINE LEARNING)
https://drive.google.com/file/d/1pQxtljlNVh0DHYg-Ye7dtpDTlFceHVfa/view


## STEP BY STEP PROCEDURE
1. Download the **Dataset** that is provided above (click the **link** and download it!)
2. Upload the dataset (csv format) in the google collab.
3. Import the dependencies like numpy, pandas, sklearn(model_selection (train_test_split), Liner_Model (LogisticRegression), and Metrics (for accuracy)
4. To read the csv file. Assign a variable called "sd" and then pd.read_csv('---filename---')
5. Perform basic .head(), .tail(), .describe(), .shape, [column_no].value counts,  functions to see the actions.
6. Then perform Train_Test_Split, X, Y, test_size = 0.1 means 10% and startify = Y (on which basis we are classifying), random_state = 1
7. X and Y has both Train and Test Sets
8. X = sd.drop(columns=60, axis=1) and Y = sd[60]
9. That means X has all data except 60th column and Y has the data of the 60th Column
10. X_train, X_test, Y_train, Y_test = train_test_split(X, Y, test_size=0.1, stratify=Y, random_state=1)
11. model = LogisticRegression()    We are training the Model with Logistic Regression
12. model.fit(X_train, Y_train)     We will be fitting the data in the form of X_train and Y_train
13. X_train_prediction = model.predict(X_train)    training_data_accuracy = accuracy_score(X_train_prediction, Y_train)
14. {Predicting the train Dataset and performing the accuracy score}
15. X_test_prediction = model.predict(X_test)      testing_data_accuracy = accuracy_score(X_test_prediction, Y_test)
16. {Predicting the test Dataset and performing the accuracy score}
17. input_data_nparray = np.asarray(input_data)
18. Changing the inout data as numpy array
19. input_data_reshaped = input_data_nparray.reshape(1,-1)
20. Reshaping of input data as numpy array was performed.
21. prediction = model.predict(input_data_reshaped)    print("Prediction - ", prediction)
22. Again Prediction is done, whether it's a Rock or Mine.
23. These include Train, Test and Validate sets.
