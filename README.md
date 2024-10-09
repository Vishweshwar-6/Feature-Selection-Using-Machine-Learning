# Feature-Selection-Using-Machine-Learning
This project demonstrates various feature selection techniques used in machine learning to identify the most relevant features in a dataset. Feature selection is a critical step in building machine learning models, as it helps improve model performance by reducing dimensionality, mitigating overfitting, and enhancing interpretability.

# Table of Contents
  - **Introduction**
  - **Feature Selection Techniques**
    - **Filter Methods**
    - **Wrapper Methods**
    - **Embedded Methods**
  - **Project Structure**
  - **Dependencies**
  - **License**

# Introduction
  Feature selection is the process of selecting a subset of the most important variables from a dataset to build a machine learning model. This project provides an implementation of various feature selection methods in Python, using a dataset to demonstrate the advantages and limitations of each method.

# By selecting the right set of features, we aim to:

  - **Improve model accuracy**
  - **Reduce computational costs**
  - **Prevent overfitting**
  - **Simplify the model for better interpretability**
  - **Feature Selection Techniques**
  
In this project, the following feature selection methods are explored:

# 1. Filter Methods
  Filter methods rank features based on statistical measures and select the top features according to their score. These methods are fast and efficient but are univariate, meaning they don't consider interactions between features. Some common filter methods implemented in this project include:
  
  **Correlation Coefficient**: Measures the linear relationship between features and the target variable.
  
  **Chi-Square Test**: A statistical test applied to categorical variables to assess the independence of two variables.
  
  **Variance Threshold**: Removes features with low variance across samples, assuming that low variance indicates little information.

# 2. Wrapper Methods
  Wrapper methods evaluate subsets of features by training models on different combinations of features. These methods are more computationally expensive but provide better feature subsets than filter methods because they consider feature interactions. Implemented wrapper methods include:
  
  **Recursive Feature Elimination (RFE)**: This method recursively removes the least important features and builds the model on the remaining subset of features.
  
  **Forward Selection**: Starts with an empty model and adds features one by one, based on which one improves the model performance the most.
  
  **Backward Elimination**: Starts with all the features and removes the least important features step by step, based on model performance.
  
# 3. Embedded Methods
  Embedded methods combine the advantages of both filter and wrapper methods. They use algorithms that have built-in feature selection capabilities. Examples of embedded methods used in this project include:
  
  **Lasso Regression (L1 Regularization)**: Penalizes the absolute size of coefficients, shrinking some coefficients to zero, effectively performing feature selection.
  
  **Random Forest Importance**: A tree-based model that provides a feature importance score based on how useful each feature was for making decisions in the trees.
  
  **Gradient Boosting**: Another tree-based model that calculates feature importance by assessing how frequently and effectively a feature is used in decision splits.
  
# Project Structure
  The project includes the following files:
  
  **CE 556 Feature Selection.ipynb**: This Jupyter notebook contains all the code for performing feature selection on a dataset. It includes detailed explanations of each method and visualizations to interpret the results.
  
  **requirements.txt**: A list of the Python packages and libraries required to run the notebook.
  
  **Key Sections in the Notebook**:
  
  **Data Preprocessing**: This section covers loading and preprocessing the dataset to make it suitable for feature selection techniques. Missing values, categorical variables, and data scaling are handled here.
  
  **Feature Selection Methods**: The notebook contains code for applying various feature selection techniques (filter, wrapper, embedded) and comparing the results.
  
  **Model Evaluation**: After selecting the best subset of features, machine learning models are trained, and their performance is evaluated using metrics like accuracy, precision, recall, and F1-score.
  
  **Visualization**: The results of feature selection are visualized using bar plots, heatmaps, and other charts to understand the importance of selected features.


# Dependencies
  The following Python libraries are required and listed in requirements.txt:
  
  -**numpy**
  -**pandas**
  -**scikit-learn**
  -**matplotlib**
  -**seaborn**
  
# License
  This project is licensed under the GNU General Public License v3.0 - see the LICENSE file for details.
