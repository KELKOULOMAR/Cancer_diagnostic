# Cancer_diagnostic
Machine Learning Classification

For this project, we use the Breast Cancer Wisconsin (Diagnostic) Database to create a classifier that can help diagnose patients. First, we read through the description of the dataset.

### 1st step:
We convert the dataset to a DataFrame to help make many things easier such as munging data.

### 2nd step:
We calcuate the class distribution (i.e. how many instances of `malignant` (encoded 0) and how many `benign` (encoded 1))

### 3rd step:
We split the DataFrame into `X` (the data) and `y` (the labels).
Then, Using `train_test_split`, we split `X` and `y` into training and test sets `(X_train, X_test, y_train, and y_test)`.
Using KNeighborsClassifier, we fit a k-nearest neighbors (knn) classifier with `X_train`, `y_train` and using one nearest neighbor (`n_neighbors = 1`)

### 4th step:
Using our knn classifier, we predict the class label using the mean value for each feature.

### 5th step:
Find the score (mean accuracy) of our knn classifier using `X_test` and `y_test`.

### 6th step:
Using the plotting function we visualize the different predicition scores between training and test sets, as well as malignant and benign cells.
