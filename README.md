In this lab, pipelines were implemented using scikit-learn to simplify machine learning workflows on the Wine Quality dataset. The dataset was first explored to observe that the features were on different scales, making feature scaling necessary for distance-based algorithms such as K-Nearest Neighbors (KNN).

The data was divided into predictor variables (X) and the target variable (y), followed by splitting the dataset into training and testing sets to prevent data leakage. Feature standardization was then performed using StandardScaler().

A KNN classifier was initially trained using a manual workflow where scaling and model training were done separately. The model achieved an accuracy of 0.5775 on the test set.

Next, a pipeline was created combining StandardScaler() and KNeighborsClassifier(). The pipeline automated preprocessing and model fitting in a single workflow while producing the same accuracy score of 0.5775.

The lab further demonstrated how pipelines can be integrated with GridSearchCV() by building a second pipeline containing StandardScaler() and RandomForestClassifier(). Hyperparameter tuning was performed using cross-validation, resulting in an improved test accuracy of 0.6075.

Overall, the lab highlighted the importance of pipelines in reducing repetitive code, preventing preprocessing errors, avoiding data leakage, and simplifying hyperparameter tuning in machine learning projects.


