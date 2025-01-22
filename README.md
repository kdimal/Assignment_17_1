_**Overview**_

This repository contains a commparison of the following classifiers: K Nearest Neighbor, Logistic Regression, Decision Trees, and Support Vector Machines. The data utilized came from the UCI repository, which represents marketing campaigns for a Portuguese bank. Specifically, it contains 41,188 records related to multiple direct telemarketing campaigns. The goal is to predict if a client will subscribe to a term deposit (target variable y).  https://archive.ics.uci.edu/dataset/222/bank+marketing

Link to Jupyter Notebook: https://codio.com/kdimal178136121/module-17-1/tree/prompt_III.ipynb

_**Model Performance Summary**_

After evaluating the performance of four different classifiers—Logistic Regression, K-Nearest Neighbors (KNN), Decision Tree, and Support Vector Machine (SVM):

**Logistic Regression**
Train Time: 1.54 seconds (fast)
Train Accuracy: 90.15%
Test Accuracy: 89.63%
Takeaway: Logistic Regression strikes an excellent balance between speed and performance, making it a reliable and efficient choice. It generalizes well to unseen data.

**KNN**
Train Time: 7.06 seconds (relatively slow due to neighbor lookups)
Train Accuracy: 91.47%
Test Accuracy: 88.83%
Takeaway: KNN has good training accuracy but slightly lower test accuracy, hinting at mild overfitting. Its slower training time could make it less ideal for large datasets.

**Decision Tree**
Train Time: 0.36 seconds (very fast)
Train Accuracy: 99.54%
Test Accuracy: 83.75%
Takeaway: Decision Trees fit the training data almost perfectly, but the much lower test accuracy indicates significant overfitting. This model would benefit from hyperparameter tuning (e.g., limiting tree depth).

**SVM (Support Vector Machine)**
Train Time: 63.25 seconds (very slow)
Train Accuracy: 89.82%
Test Accuracy: 89.48%
Takeaway: SVM delivers solid accuracy but comes with a high computational cost. This might be suitable for smaller datasets or where high accuracy is paramount and computation time is less critical.

_**Overall Insights**_

_Best All-Rounder:_ Logistic Regression offers the best balance between speed, training accuracy, and test accuracy.

_Overfitting Issues:_ Decision Tree significantly overfits the training data, making it less suitable without tuning.

_Costly but Effective:_ SVM provides comparable accuracy to Logistic Regression but at a much higher computational expense.

_KNN's Trade-off:_ While KNN performs well, its slower training time makes it less scalable for larger datasets.

_**Recommendation**_

For most practical applications, Logistic Regression is the most efficient and reliable choice. If computational cost isn’t a concern, SVM is a close contender. Further tuning could improve the performance of KNN and Decision Tree, but Logistic Regression remains the most balanced option for this dataset.
