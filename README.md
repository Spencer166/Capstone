**Summary**

Credit risk assessment is essential for minimizing loan defaults and financial loss for both borrower and lender. This project develops an end-to-end machine learning solution to predict the likelihood of loan default using historical borrower and loan data. Multiple classification models were evaluated using a GridSearch. Ultimately, a gradient boosting model was selected based on a strong performance with metrics ROC-AUC and accuracy. The final model was deployed as a prediction service using a Flask API, containerized with Docker and hosted on AWS. This project demonstrates a practical, production-oriented approach to building and deploying a credit risk model that can be monitored, retrained and scaled as new data becomes available.


**Application Instructions**

1. Click this link to open the appication: http://credit-risk-balancer-301773526.us-east-2.elb.amazonaws.com:5000/
2. For the fields Annual Income, Debt-to-Income Ratio, Credit Score, Loan Amount, Interest Rate: Type the correct metric for each field. Note: this app will not accept inputs with more than 2 decimal places.
3. For the fields Gender, Marital Status, Education Level, Employment Status, Loan Purpose: Use the dropdowns to select the right category for each.
4. For the Grade/Subgrade field: Type the appropriate grade for the loan (e.g., A1, B2, B3, C3).
5. Click the "Predict Credit Risk" button.
6. The app will return two different results: Prediction: This is a binary prediction of whether the borrower will pay back the loan or not (Repay or Default). Payback Probabity: Ths is the probability that the borrower will payback the loan.
