# 📂 Week 4: Regression Models and Model Optimization

# 📅 Day 13: Linear, Ridge, and Lasso Regression

**Date:** July 20, 2026

### 📝 Technical Competencies Acquired

#### 1. Introduction to Regression Analysis
* Developed an understanding of regression as a supervised machine learning technique used for predicting continuous numerical values.
* Learned how regression models establish relationships between independent features and a target variable.
* Understood the applications of regression in predictive analytics and decision-making.

#### 2. Linear Regression
* Studied Linear Regression as a fundamental regression algorithm that fits the best possible linear relationship between input features and the target variable.
* Learned how Linear Regression estimates predictions using a best-fit line.
* Understood the advantages and limitations of Linear Regression when dealing with complex datasets.

#### 3. Ridge Regression
* Explored Ridge Regression as a regularized version of Linear Regression.
* Learned how Ridge Regression introduces an L2 penalty to reduce model complexity and prevent overfitting.
* Understood how coefficient shrinkage improves model generalization while retaining all input features.

#### 4. Lasso Regression
* Studied Lasso Regression as a feature selection and regularization technique.
* Learned how Lasso applies an L1 penalty that reduces the coefficients of less significant features to zero.
* Understood the importance of Lasso in simplifying models and selecting the most influential predictors.

#### 5. Model Regularization
* Developed an understanding of regularization techniques for controlling model complexity.
* Compared L1 and L2 regularization methods and their effects on feature coefficients.
* Learned how regularization improves model stability and predictive performance on unseen data.

#### 6. Comparative Analysis of Regression Models
* Compared Linear Regression, Ridge Regression, and Lasso Regression based on prediction accuracy and model behavior.
* Understood the strengths, limitations, and practical use cases of each regression technique.
* Learned how different regression algorithms respond to datasets containing multiple predictive features.

---

### 💻 Practical Implementations

* Imported the Teen Mental Health dataset using Pandas.
* Selected relevant predictive features, including:
    * Daily Social Media Hours
    * Sleep Hours
    * Academic Performance
    * Stress Level
    * Anxiety Level
    * Addiction Level
* Split the dataset into training and testing subsets using `train_test_split()`.
* Implemented a Linear Regression model using Scikit-learn.
* Applied Ridge Regression with L2 regularization.
* Applied Lasso Regression with L1 regularization.
* Generated predictions for both testing data and new sample inputs.
* Converted regression outputs into binary class predictions using thresholding for comparison.
* Evaluated model performance using Accuracy Score.
* Created a comparison table summarizing the performance of all three regression models.

---

### 📚 Learning Outcomes

* Developed a strong understanding of regression-based supervised learning techniques.
* Learned the working principles of Linear Regression, Ridge Regression, and Lasso Regression.
* Acquired practical experience in implementing regression models using the Scikit-learn library.
* Improved understanding of L1 and L2 regularization techniques and their importance in preventing overfitting.
* Learned how feature selection can improve model simplicity and interpretability through Lasso Regression.
* Gained experience in comparing multiple regression models based on their predictive performance.
* Enhanced proficiency in preparing datasets, training regression models, and generating predictions.
* Established a strong foundation for advanced regression techniques and model optimization methods.

---

⭐ ⭐ ⭐

---

# 📅 Day 16: Feature Selection Techniques for Machine Learning

**Date:** July 21, 2026

### 📝 Technical Competencies Acquired

#### 1. Introduction to Feature Selection
* Developed an understanding of **Feature Selection** as the process of selecting the most relevant features from a dataset while eliminating redundant and less informative attributes.
* Learned how feature selection improves machine learning model efficiency, interpretability, and predictive performance.
* Understood the importance of reducing dataset dimensionality before model training.

#### 2. Benefits of Feature Selection
* Studied the advantages of feature selection in machine learning workflows, including:
    * Faster model training.
    * Improved prediction accuracy.
    * Reduced risk of overfitting.
    * Lower memory consumption.
    * Better model interpretability.
    * Removal of irrelevant and redundant features.

#### 3. Types of Feature Selection Methods
* Explored the three primary categories of feature selection techniques:
    * **Filter Methods**
    * **Wrapper Methods**
    * **Embedded Methods**
* Understood the differences between these approaches and their applications in machine learning.

#### 4. Variance Threshold Method
* Studied the Variance Threshold technique for identifying and removing features with very low variance.
* Learned how nearly constant features contribute minimal information during model training.
* Understood the importance of selecting an appropriate variance threshold for effective feature reduction.

#### 5. Correlation-Based Feature Selection
* Explored correlation analysis as a method for measuring the relationship between input features and the target variable.
* Learned how features with stronger correlations often provide greater predictive value.
* Visualized feature relationships using a correlation heatmap.

#### 6. Chi-Square Feature Selection
* Studied the Chi-Square statistical test for evaluating the dependency between categorical features and the target variable.
* Learned how higher Chi-Square scores indicate stronger relationships with the target.
* Understood the suitability of the Chi-Square test for classification problems.

#### 7. Mutual Information
* Developed an understanding of Mutual Information as a feature selection technique capable of identifying both linear and non-linear relationships.
* Learned how Mutual Information measures the amount of information shared between a feature and the target variable.
* Understood its importance in selecting informative features for predictive modeling.

---

### 💻 Practical Implementations

* Imported the Teen Mental Health dataset using Pandas.
* Encoded categorical features using `LabelEncoder`.
* Applied Variance Threshold to remove low-variance features.
* Calculated feature variances and visualized them using Matplotlib bar charts.
* Performed correlation analysis between input features and the target variable.
* Generated a correlation heatmap using Seaborn.
* Implemented Chi-Square feature selection using `SelectKBest` and `chi2`.
* Applied feature scaling using `MinMaxScaler` before Chi-Square analysis.
* Calculated Mutual Information scores using Scikit-learn.
* Compared feature importance rankings obtained from multiple feature selection techniques.

---

### 📚 Learning Outcomes

* Developed a strong understanding of the importance of feature selection in machine learning pipelines.
* Learned how removing irrelevant and redundant features improves model efficiency and generalization.
* Gained practical experience with Variance Threshold, Correlation Analysis, Chi-Square, and Mutual Information feature selection techniques.
* Improved understanding of statistical methods used for identifying important predictive variables.
* Acquired proficiency in using Scikit-learn's feature selection modules for preprocessing tasks.
* Learned how to visualize feature importance using bar charts and correlation heatmaps.
* Enhanced the ability to compare different feature selection techniques based on dataset characteristics.
* Established a strong foundation for building efficient, interpretable, and high-performing machine learning models.
---

⭐ ⭐ ⭐

---

# 📅 Day 17: Wrapper-Based Feature Selection Techniques

**Date:** July 22, 2026

### 📝 Technical Competencies Acquired

#### 1. Introduction to Wrapper Methods
* Developed an understanding of **Wrapper Methods** as feature selection techniques that evaluate different subsets of features using a machine learning model.
* Learned how wrapper methods determine the optimal combination of features based on model performance rather than statistical measures alone.
* Understood the advantages of wrapper methods in improving prediction accuracy through informed feature selection.

#### 2. Forward Feature Selection
* Studied Forward Selection as an iterative feature selection technique.
* Learned how the algorithm starts with an empty feature set and progressively adds features that provide the greatest improvement in model performance.
* Understood the stopping criteria based on the desired number of selected features or performance improvement.

#### 3. Backward Feature Elimination
* Explored Backward Elimination as a reverse feature selection approach.
* Learned how the algorithm begins with all available features and removes the least significant feature at each iteration.
* Understood how eliminating unnecessary features simplifies the model while maintaining predictive performance.

#### 4. Recursive Feature Elimination (RFE)
* Studied Recursive Feature Elimination (RFE) as an embedded wrapper technique.
* Learned how RFE repeatedly trains a model, ranks feature importance, and removes the least important features until the desired number of predictors remains.
* Understood the importance of feature ranking in selecting the most informative variables.

#### 5. Recursive Feature Elimination with Cross Validation (RFECV)
* Developed an understanding of RFECV as an enhanced version of RFE.
* Learned how cross-validation automatically determines the optimal number of features by evaluating model performance across multiple folds.
* Understood the advantages of RFECV in selecting an optimal feature subset while reducing the risk of overfitting.

#### 6. Model-Based Feature Selection
* Explored the use of Logistic Regression and Decision Tree classifiers for evaluating feature subsets.
* Learned how different machine learning algorithms may select different feature combinations based on their learning mechanisms.
* Understood the relationship between feature selection and model performance.

---

### 💻 Practical Implementations

* Imported the Teen Mental Health dataset using Pandas.
* Encoded categorical variables using `LabelEncoder`.
* Separated the dataset into input features and target variables.
* Implemented **Forward Feature Selection** using `SequentialFeatureSelector`.
* Applied **Backward Feature Elimination** to identify the most relevant predictors.
* Performed **Recursive Feature Elimination (RFE)** using Logistic Regression.
* Generated feature rankings based on model importance.
* Implemented **RFECV** to automatically determine the optimal number of features using cross-validation.
* Compared the feature subsets selected by different wrapper-based feature selection techniques.

---

### 📚 Learning Outcomes

* Developed a strong understanding of wrapper-based feature selection methods and their significance in machine learning.
* Learned how Forward Selection, Backward Elimination, RFE, and RFECV identify the most informative features.
* Acquired practical experience in implementing feature selection techniques using Scikit-learn and Mlxtend.
* Improved understanding of how feature selection contributes to better model accuracy and reduced computational complexity.
* Gained knowledge of feature ranking and model-based evaluation strategies.
* Learned the importance of cross-validation in selecting the optimal number of predictive features.
* Enhanced proficiency in preprocessing datasets and optimizing feature subsets for supervised learning models.
* Established a strong foundation for advanced feature engineering and machine learning model optimization.

---
