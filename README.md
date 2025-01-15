# Developing Loan Default Prediction Model for Fairness and Accuracy
This project tackles a critical challenge in the financial sector: credit default prediction. It prioritizes building a model that is not only accurate in predicting loan defaults, but also fair and unbiased in its outcomes, particularly regarding gender. This was achieved through innovative techniques, specifically using XGBoost and Fairlearn's ThresholdOptimizer to minimize gender bias in the model's predictions. The project's success was recognized by its **1st place** win at the **Enigma Hackathon**, held within Codefest'24 at IIT BHU.

**Model Used:**

* XGBoost: A powerful gradient boosting algorithm known for its effectiveness in credit risk prediction tasks.

**Key Points:**

* **Fairness Integration:** Fairlearn's ThresholdOptimizer ensures demographic parity for gender during model training. This helps to mitigate potential bias in the model's predictions and prevent discriminatory outcomes based on gender.
* **Hyperparameter Tuning:** The code utilizes Hyperopt for hyperparameter tuning with Stratified K-Fold Cross-Validation. This process optimizes the model's performance while maintaining fairness.
* **Preprocessing and Evaluation:** The code incorporates data preprocessing steps like handling missing values and encoding categorical features. Additionally, it evaluates the model's performance using metrics like F1-score and Demographic Parity Ratio (DPR) for gender.


**Results:**

The script outputs the following key results to assess the model's performance and fairness:

* **F1-score:**  **0.5342**. This metric indicates a good balance between precision and recall in predicting loan defaults.
* **Demographic Parity Ratio (DPR) for Gender:** **0.9799**. This value close to 1 signifies a high level of fairness achieved by the model. In simpler terms, the model predicts loan defaults at similar rates for both genders, mitigating potential gender bias.

The predictions of the model are stored [here](https://github.com/Dream-Falls/Enigma/blob/main/submission.csv).
