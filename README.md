** Customer Churn Prediction – Beta Bank
* Problem

Customer churn is a critical issue in the banking sector, as losing clients directly impacts revenue.
The goal of this project is to build a machine learning model capable of predicting whether a customer will leave the bank, enabling proactive retention strategies.

* Data

The dataset contains customer-related features such as:

Demographics (age, geography, gender)
Account information (balance, tenure, number of products)
Activity indicators (credit card usage, active membership)

The data presented class imbalance, which required additional preprocessing techniques.

* Approach

The project followed a structured machine learning workflow:

Data cleaning and preprocessing
Exploratory Data Analysis (EDA)
Feature engineering
Model training and evaluation

Several models were tested:

Logistic Regression
Decision Tree
Random Forest

To address class imbalance, both upsampling and downsampling techniques were applied.

* Results

The best-performing model was Random Forest with upsampling, achieving:

F1 Score: 0.626
ROC AUC: 0.856

Other key results:

Random Forest (baseline): F1 = 0.601, ROC AUC = 0.850
Downsampling models improved recall but reduced precision
Logistic Regression showed lower performance overall
Decision Trees performed moderately but were less stable than ensemble methods

The ROC curve demonstrated strong classification capability, indicating a good balance between true positive and false positive rates.

* Conclusion

The Random Forest model with upsampling proved to be the most effective approach for predicting customer churn. It achieved the best balance between precision and recall, while maintaining strong discriminative power.

This model is a robust solution for churn prediction under imbalanced data conditions and aligns with the project goal of optimizing F1 Score without sacrificing overall performance.

* Tools & Technologies
Python
Pandas, NumPy
Scikit-learn
Matplotlib / Seaborn

*** This project demonstrates the application of machine learning techniques to solve a real-world business problem, with a focus on model performance and interpretability.
