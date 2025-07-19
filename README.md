# logistic-gd-mnist
实现带 L2 正则和回溯线搜索的逻辑回归

The gradient  is crucial in the gradient descent (GD) algorithm. You need first calculate .
The choice of the step size  in GD is also very important. It affects the efficiency of GD. However, the exact line search is not available for  in logistic regression. Instead, we may use a simple backtracking line search with the Armijo–Goldstein condition. Read and understand this strategy at https://en.wikipedia.org/wiki/Backtracking_line_search.
The choice of the regularization parameter  in the function  is also crucial. It affects the performance of logistic regression quite much. We may use Leave-One-Out Cross-Validation for tuning . Search online and understand leave-one-out cross-validation.
Test your logistic regression on the MNIST dataset, which is downloaded at https://www.kaggle.com/datasets/oddrationale/mnist-in-csv?resource=download.
We randomly pick 1000 examples with label "3" and 1000 examples with label "8" from mnist_train.csv as the training dataset, where the labels 3 and 8 are re-labeled as class -1 and +1 respectively.
Use GD with backtracking line search and Leave-One-Out Cross-Validation to train your logistic regression model.
Upload your code, and report the success rate of the prediction of labels for samples in mnist_test.csv with labels 3 and 8.
Write a report on this project. Your report may contain (but is not limited to) an algorithm description, the experimental settings, the results, and a discussion on possible improvements to the algorithms.
