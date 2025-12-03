**Overview**

This repository contains the machine learning component of my study on the determinants of student performance using the NELS:88 longitudinal dataset. I apply supervised regression models, supervised classification models, and unsupervised learning techniques (PCA and K-Means) to examine how class size, demographics, and teacher characteristics relate to academic outcomes.
My goal is to complement traditional econometric methods with modern ML techniques for prediction, pattern detection, and feature importance analysis.

**Dataset**

I work with cleaned student-, teacher-, and school-level data from the NELS:88 survey.
Key features include:
1. Student demographics
2. Family income
3. Teacher certification and full-time status
4. Absenteeism and aspirations
5. Class-size variables
6. Composite test scores (1988, 1990, 1992)

**Supervised Learning: Regression Models**

I train several regression models to predict log total test scores (ln_totalscr92):
1. Linear Regression
2. LASSO and Ridge
3. Random Forest Regressor
4. Gradient Boosted Trees
5. KNN Regression

**Findings**

Tree-based models achieve the lowest RMSE.

Feature importance consistently highlights family income, prior scores, and aspirations as dominant predictors.

Class size contributes minimally and ranks low across all models.

**Supervised Learning: Classification Models**

I analyse two binary outcomes:
1. absent88_bin — whether the student was frequently absent
2. uni_aspire88 — whether the student aspires to complete university

**Models used:**
1. Logistic Regression
2. Random Forest
3. Gradient Boosting
4. KNN
5. SVM

**Findings**

Gradient Boosting and Random Forests produce the highest AUC.

Socioeconomic and prior-achievement variables strongly influence predictions.

Class-size indicators again have limited predictive value.

**Unsupervised Learning: PCA & K-Means**

1. PCA - reduces dimensionality while retaining most variance. First two components cluster strongly by SES and prior academic performance.
2. K-Means - students cluster into low-, medium-, and high-achievement groups. Clusters are driven primarily by socioeconomic status and early test scores rather than class size.


**Key Takeaways**

ML results reinforce the econometric findings: class size has limited predictive power compared to SES and prior academic performance.
Ensemble models outperform linear models across regression and classification tasks.
PCA and K-Means reveal clear underlying structure shaped by socioeconomic background.

**Contact**

You can reach me at rangi.ho@gmail.com if you would like to verify the results or request a copy of the paper.
