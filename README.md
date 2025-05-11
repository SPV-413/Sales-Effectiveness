# Sales Effectiveness
FicZon Inc, a provider of on-premises and SaaS IT solutions, is experiencing a drop in sales due to rising competition and reliance on manual lead categorization. The current process is subjective and delays decision-making, as it depends heavily on sales staff experience. Although a quality check exists, it is only useful for post-sale analysis. To improve sales efficiency and conversion rates, FicZon plans to implement a Machine Learning model that can automatically classify leads as "High Potential" or "Low Potential" at the time they are created, enabling sales teams to focus on the most promising opportunities.

## Dataset Overview
- **Source**: DataMites
- **Rows**: 7422
- **Columns**: 9 (including the target variable)
- **Target Variable**: 
  - Status
- **Features**:
  - Created
  - Product_ID
  - Source
  - Mobile
  - EMAIL
  - Sales_Agent
  - Location
  - Delivery_Mode

## Project Workflow
### 1. Exploratory Data Analysis (EDA)
- Data loading
- Data visualization using Matplotlib & Seaborn
### 2. Feature Engineering
- Map 'Status' to High/Low potential
- Handle datetime (Created)
- Create New Features
- Drop unrequired columns
- Check unique values
- Imputation for Empty Strings
- Check null values
- Removing duplicates
- Identifying & Handling the outliers(`Boxplot & Winsorize`)
- Checking Skewness
- Encoding categorical features(`LabelEncoder`)
- Feature selection
- Feature scaling(`MinMaxScaler`)
- Splitting dataset into training & testing sets(`train_test_split`)
- Feature Balancing(`SMOTE`)

  
### 3. Machine Learning Models
The project implements multiple machine learning models & one deep learning model for classification:
- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- Gradient Boosting Classifier
- XGBoost Classifier
- K-Neighbors Classifier(KNN)
- Support Vector Classifier(SVC)
- Multi-layer Perceptron (MLP) Classifier

### 4. Hyperparameter Tuning
- GridSearchCV is used to optimize model parameters.

### 5. Model Evaluation
- Accuracy Score
- Confusion Matrix
- Classification Report

## Installation & Usage

### Prerequisites
Ensure you have the following installed:
- Python 3.10 and above
- Jupyter Notebook
- Required libraries (`pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`)

### Running the Notebook
1. Clone the repository:
   git clone https://github.com/SPV-413/Sales-Effectiveness.git
2. Navigate to the project folder:
   cd Sales-Effectiveness
3. Open the Jupyter Notebook:
   jupyter notebook PRCL-0019-Sales Effectiveness.ipynb

## Conclusion
- The **Gradient Boosting** achieved the highest accuracy score (0.71), making it the **most effective model** among those evaluated.
- Ensemble methods like **Random Forest**, **XGBoost** and **Gradient Boosting** consistently outperformed traditional models, showing their strength in handling complex patterns.
- By strategically focusing on the insights revealed through Data Exploration, result in a significant boost in sales effectiveness.

## Contact
For any inquiries, reach out via GitHub or email.
