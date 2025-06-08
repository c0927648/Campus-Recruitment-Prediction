# Campus-Recruitment-Prediction

In this project, the goal was to predict whether a student would be placed or not using various machine learning models. We began by performing exploratory data analysis (EDA) and preprocessing, including handling missing values, encoding categorical variables, and splitting the data into training and test sets with stratified sampling due to class imbalance.

Three models were trained and tuned using GridSearchCV: Logistic Regression, Random Forest, and Support Vector Machine (SVM). Each model was evaluated using accuracy, precision, recall, F1-score, and confusion matrices. Random Forest achieved the best performance overall, particularly in identifying both placed and not placed students.

A soft voting ensemble was then built to combine the strengths of all three models. While the Voting Classifier maintained high recall for placed students, it did not improve performance on the minority class compared to Random Forest alone.

Finally, predictions were generated on an unseen test dataset using the trained Random Forest model, after aligning the features appropriately.
