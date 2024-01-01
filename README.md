# Kids Hobby Prediction using R language

## Problem
Children often face uncertainty when exploring their interests, whether in academics, arts, or sports. To aid parents in guiding their children towards activities they are passionate about, we've gathered a dataset from parental surveys. This dataset contains valuable information to build a classification model predicting children’s hobbies.

## Data Preprocessing
### 1-Data Cleaning:
Cleaning up data means fixing any mistakes, inconsistencies, or errors in the dataset. It makes the data more trustworthy for analysis and modeling. We checked for missing values, outliers, and issues, but didn't find any in our dataset.

### 2-Encoding:
Encoding is about turning non-number information into numbers so the computer can understand it better for later steps.

### 3-Normalization and Discretization:
We didn't need to normalize or discretize our data because it doesn't have the kind of information that needs these adjustments. Doing these things could make mistakes or create false relationships in our data.

### 4-Feature Selection:
To make our predictions more accurate and faster, we're picking the most important parts from our data. This way, we're only using what really matters for predicting hobbies. We're using methods like Rank Features by Importance and Feature Selection Using Recursive Feature Elimination (RFE) to do this.

## Data Mining Technique
### 1-Classification Technique:
Explored attribute selection's role in building robust models for accurate predictions.
Examined model performance across different data splits (e.g., “90%”, “10%”) for adaptability.
Implemented Information Gain, Gini Index, and Gain Ratio via 'rpart' in R to optimize decision trees.

### 2-Clustering Techniques:
Chose k-medoids (PAM) over k-means for categorical data suitability.
Preprocessed data (converted, scaled) and determined optimal clusters (k=3) using validation methods.
Evaluated metrics (BCubed recall, precision, silhouette width) to finalize k=3 as the best cluster count.
