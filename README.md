# Bayesian_network

This project uses Bayesian Networks to predict the occurrence of heart disease based on certain risk factors.

# Data
The data used in this project is a set of medical records for different patients. Each record includes:

Age: Discretized into the categories 0-12, 13-20, 21-35, 36-50, 50-60, and 60-100.
Heart Disease: Binary outcome - 0 for no heart disease, 1 for presence of heart disease.
Blood Pressure: Discretized into two categories - 'normal' (0-135) and 'high' (136-200).
Cholesterol: Discretized into two categories - 'normal' (0-300) and 'high' (300-400).
Model
We used a Bayesian Network to model the joint probability distribution of the data. The network was trained using the Hill-Climb Search algorithm with the BIC score as the scoring function.

The model's structure represents the dependencies among variables. The conditional probability distribution (CPD) of each variable, given its parents in the network, was estimated using Maximum Likelihood Estimation.

# Analysis and Results
We examined the estimated CPDs to understand the relationships among variables. We performed variable elimination to carry out inference queries, which helped us understand the effect of different factors on the probability of heart disease.

For instance, we could query the model to find out the probability of heart disease given a patient's age, blood pressure, and cholesterol level. This provides a quantitative way of understanding how different factors contribute to heart disease risk.

# Evaluation
We evaluated the model's performance by generating predictions for a held-out test set and comparing them to the actual outcomes. The performance was quantified using a confusion matrix, which provides a breakdown of true positives, true negatives, false positives, and false negatives.

