# Deep Learning Binary Classification with TensorFlow

## Project Overview
This repository contains an applied deep learning project that uses TensorFlow to build a binary classification neural network on a social network advertising dataset. The objective is to predict whether a user will purchase a product based on demographic features, demonstrating an end-to-end deep learning workflow from preprocessing through evaluation.

---

## Business Problem
In digital marketing and paid media, identifying users most likely to convert is critical for optimizing spend and personalization strategies. This project frames the problem as a **customer propensity modeling task**, predicting purchase likelihood using demographic signals commonly available in advertising platforms.

---

## Dataset
The dataset (`Social_Network_Ads.csv`) contains user-level advertising data with the following features:
- **Age**
- **Estimated Salary**
- **Purchased** (binary target variable)

Each record represents a potential customer exposed to advertising, with the target indicating whether a purchase occurred.

---

## Data Preprocessing
To prepare the data for modeling:
- Numeric features were standardized to improve neural network training stability
- The dataset was split into training and test sets
- Features and labels were validated for correct data types and shape

These steps ensured consistent model convergence and generalization.

---

## Model Architecture
A feed-forward neural network was built using TensorFlow:
- Input layer corresponding to demographic features
- One or more hidden layers with nonlinear activation functions
- Output layer with a sigmoid activation function for binary classification

The architecture balances simplicity with expressive power given the dataset size.

---

## Model Training and Evaluation
The model was trained using:
- Binary cross-entropy loss
- Adaptive optimization (e.g., Adam optimizer)
- Accuracy and confusion matrix analysis for evaluation

Performance was assessed on a held-out test set to evaluate generalization.

---

## Overall Findings
Key findings from this project include:

- **Age and estimated salary provide meaningful predictive signal**, with the model learning nonlinear decision boundaries that outperform simple linear separation.
- The neural network effectively distinguishes high-propensity purchasers from non-purchasers, particularly in regions of the feature space with clear demographic separation.
- Misclassifications tend to occur near boundary regions, highlighting the limitations of using only two demographic features without behavioral or contextual data.
- The results demonstrate how even limited feature sets can support effective propensity modeling when combined with nonlinear machine learning techniques.

These findings mirror real-world marketing analytics scenarios, where demographic data often serves as an initial signal before richer behavioral data is introduced.

---

## Limitations and Future Improvements
While the model performs well for a small dataset, several improvements could enhance real-world applicability:
- Incorporating behavioral features such as engagement or browsing history
- Hyperparameter tuning and architecture experimentation
- Comparing neural network performance against logistic regression and tree-based baselines
- Evaluating additional metrics such as precision, recall, and ROC-AUC

---

## Technologies Used
- **Python**
- **TensorFlow**
- **Pandas & NumPy**
- **Matplotlib**
- **Jupyter Notebook**

---

## Repository Structure
