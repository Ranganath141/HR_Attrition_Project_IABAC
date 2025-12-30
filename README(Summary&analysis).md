# HR_Attrition_Project_IABAC

Project Summary :

This project focused on building a data-driven predictive system to identify employees at risk of attrition using demographic, job-related, satisfaction, and experience-based attributes. Comprehensive exploratory data analysis revealed class imbalance and highlighted key factors such as job satisfaction, work-life balance, experience, and compensation as influential drivers of employee attrition. Correlation analysis and department-level insights further supported the importance of these factors in understanding employee performance stability and retention behavior.

A structured preprocessing strategy was implemented, including appropriate encoding techniques for categorical variables, standardization of numerical features, and preservation of ordinal relationships. Multiple machine learning models were evaluated, including Decision Tree, Logistic Regression, Random Forest, and XGBoost, with performance assessed using metrics aligned to business priorities rather than accuracy alone. Special emphasis was placed on recall for the minority attrition class to minimize the risk of missing potential leavers.

Logistic Regression emerged as the most suitable predictive model due to its strong interpretability, stable generalization, and superior minority-class recall. Threshold tuning was applied to further align predictions with business objectives, enabling proactive identification of high-risk employees while maintaining controlled trade-offs in precision. The final preprocessing pipeline and predictive model were saved to ensure reproducibility and future scalability.

Based on analytical insights, targeted recommendations were proposed to improve employee performance and retention, including enhancing job satisfaction, promoting work-life balance, adopting department-specific HR strategies, supporting early-career employees, and leveraging predictive insights for proactive intervention. Overall, this project demonstrates how data-driven analysis and machine learning can support informed hiring decisions, improve workforce stability, and strengthen organizational performance.

Analysis of the project (workflow) :

The objective of this project was to build a predictive model to identify employees at risk of attrition, supporting data-driven hiring and retention decisions. Exploratory Data Analysis (EDA) was conducted to understand data distribution, class imbalance, and relationships between employee attributes and attrition. Correlation analysis indicated that job satisfaction, work-life balance, experience-related features, and compensation factors showed notable association with attrition, guiding feature selection and modeling decisions.

Categorical features were handled using appropriate encoding strategies: nominal variables such as department, job role, marital status, gender, and business travel frequency were encoded using One-Hot Encoding, while binary variables like overtime were ordinally encoded. Ordinal and score-based features, including satisfaction ratings, job level, performance rating, and work-life balance, were passed through without transformation to preserve their inherent ordering. Numerical features with varying scales were standardized to improve model stability.

Multiple machine learning algorithms were evaluated, including Decision Tree, Logistic Regression, Random Forest, and XGBoost. A tuned Decision Tree provided a stable baseline, while Logistic Regression demonstrated strong interpretability and consistent performance on imbalanced data. Class imbalance was primarily handled using class weighting, and threshold tuning was applied to Logistic Regression to improve recall for the minority attrition class in alignment with business priorities. Although ensemble models such as Random Forest and XGBoost achieved higher accuracy, they underperformed in minority-class recall, making them less suitable for the project objective.

Model evaluation emphasized recall for the minority attrition class, F1-score, and confusion matrix analysis rather than accuracy alone. Logistic Regression with threshold tuning achieved the best balance between interpretability, generalization, and business relevance. The final preprocessing logic was saved using a serialized preprocessor (.pkl) file, and the trained predictive model was stored for reuse, ensuring reproducibility and consistent inference on new data.

Overall, the project followed a structured pattern.
