# SVMClassification

Steps Performed

1. Data Loading & Preparation

  Loaded the dataset breast-cancer.csv.

  Encoded the target variable diagnosis (Malignant = 1, Benign = 0).

  Removed the id column as it is not useful for training.

  Applied StandardScaler to normalize feature values.

  Split the dataset into train (80%) and test (20%) sets.

2. Training SVM Models

  Trained two SVM classifiers:

  Linear Kernel SVM (kernel='linear').

  RBF Kernel SVM (kernel='rbf').

  Evaluated accuracy of both models on the test set.

3. Decision Boundary Visualization

  Used Principal Component Analysis (PCA) to reduce dataset dimensions to 2D.

  Trained an SVM with RBF kernel on the reduced dataset.

  Visualized the decision boundary to show separation of classes.

4. Hyperparameter Tuning

  Performed hyperparameter tuning using GridSearchCV.

  Tuned parameters:

  C (regularization strength).

  gamma (influence of a single training example).

  kernel (focused on RBF).

  Found the best parameter combination and reported the best cross-validation score.

5. Model Evaluation

  Used cross-validation with 5 folds.

  Calculated accuracy for each fold.

  Reported the mean cross-validation accuracy.
