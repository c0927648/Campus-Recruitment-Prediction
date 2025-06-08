# Campus-Recruitment-Prediction

In this project, the objective was to predict whether a student would be placed or not using classical supervised machine learning techniques. We began with exploratory data analysis (EDA) to understand feature distributions, class imbalance, and data quality. Missing values were handled, categorical features were encoded using one-hot and label encoding, and a stratified train-test split was used to preserve class ratios.

Three classification models were selected and trained: Logistic Regression, Random Forest, and Support Vector Machine (SVM). Each model underwent hyperparameter tuning using GridSearchCV to optimize performance. Model evaluation was conducted using accuracy, precision, recall, F1-score, and confusion matrices. Random Forest performed best overall, with strong results in both majority and minority class predictions.

A soft Voting Classifier was then created by combining all three tuned models. While it achieved high recall on the majority class, it did not outperform Random Forest in overall metrics or in handling the minority class.

A test dataset was available but only included limited features (sl_no, gender, and salary). Since it lacked the full set of features used during model training, it was not possible to generate valid predictions from it. As a result, final deployment-level inference was not completed.
