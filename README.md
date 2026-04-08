💳 Loan Default Prediction using Artificial Neural Networks (ANN)
📌 Project Overview

This project builds an Artificial Neural Network (ANN) model to predict whether a borrower is likely to default on a loan. The dataset is sourced from LendingClub and contains real-world loan application and repayment data.

The goal is to help financial institutions minimize risk by identifying high-risk borrowers using deep learning techniques.

📊 Dataset
Source: Lending Club Loan Data
Contains:
Loan details (amount, term, interest rate)
Borrower information (income, employment, credit history)
Loan status (Fully Paid / Charged Off)

⚙️ Project Workflow
1. Data Preprocessing
Removed irrelevant columns (IDs, URLs, etc.)
Handled missing values
Converted categorical features using:
Label Encoding
One-Hot Encoding
2. Feature Engineering
Created meaningful features:
Debt-to-Income ratios
Credit utilization indicators
Scaled numerical features using Standardization
3. Exploratory Data Analysis (EDA)
Checked class imbalance (default vs non-default)
Analyzed correlations between features
Identified strong predictors:
Interest Rate
Grade
Annual Income
4. Model Building (ANN)
Built using Pytorch
Architecture:
Input Layer
Multiple Hidden Layers (ReLU activation)
Output Layer (Sigmoid activation)
5. Model Training
Loss Function: Binary Crossentropy
Optimizer: Adam
Used validation split to prevent overfitting
6. Model Evaluation
Accuracy
Precision, Recall, F1-score
Confusion Matrix

🚀 Results
ANN successfully classified loan defaults with strong performance
Improved results achieved through:
Feature scaling
Proper architecture tuning
Handling class imbalance

🧠 ANN Architecture (Example)
model = Sequential()
model.add(Dense(64, activation='relu', input_dim=X.shape[1]))
model.add(Dense(32, activation='relu'))
model.add(Dense(16, activation='relu'))
model.add(Dense(1, activation='sigmoid'))

🛠️ Tech Stack
Python 🐍
Pandas, NumPy
Scikit-learn
TensorFlow / Keras
Matplotlib, Seaborn

📂 Project Structure
├── raw.ipynb
├── accepted_2007_to_2018Q4_100k.csv
├── README.md

📈 Key Learnings
Neural networks for tabular data
Importance of feature scaling in ANN
Handling imbalanced datasets
Model tuning for better generalization

🔗 Future Improvements
Use SMOTE for class imbalance
Try Deep Neural Networks (DNN) with dropout
Compare with traditional ML models (XGBoost, Random Forest)
Deploy using Streamlit

👤 Author
Kunal Droch


## Dataset
https://www.kaggle.com/datasets/wordsforthewise/lending-club

