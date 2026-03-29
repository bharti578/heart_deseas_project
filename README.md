# Healthcare Claims Prediction Model

A machine learning project to predict denied insurance claims using healthcare data analysis and classification modeling.

## 📋 Project Overview

This project analyzes healthcare claims data to build a predictive model that identifies which claims are likely to be denied. Using exploratory data analysis and machine learning techniques, the model helps healthcare providers and insurers optimize claim processing.

## 🎯 Objectives

- Extract and clean healthcare claims data
- Perform exploratory data analysis (EDA) on patient demographics and claims
- Build a classification model to predict claim status (denied/approved)
- Identify key features influencing claim approval/denial decisions
- Save and deploy the trained model

## 📊 Dataset

The project uses `healthcare_claims_large.csv` containing:
- **Patient Information**: Age, demographics
- **Claim Details**: Claim ID, status, dates
- **Medical Information**: Treatment types, diagnoses
- **Target Variable**: Claim_Status (Denied/Approved)

## 🛠️ Technologies & Libraries

- **Python 3.x**
- **pandas** - Data manipulation and analysis
- **NumPy** - Numerical computing
- **scikit-learn** - Machine learning algorithms
- **Matplotlib** - Data visualization
- **Seaborn** - Statistical data visualization
- **joblib** - Model persistence

## 📁 Project Structure

```
├── healthcare_claims_large.csv    # Input dataset
├── heart_deseas_project.ipynb     # Main analysis notebook
├── model.pkl                      # Trained model (serialized)
└── README.md                      # This file
```

## 🚀 Workflow

### 1. **Data Loading & Exploration**
   - Load healthcare claims data using pandas
   - Display first few rows and dataset info
   - Generate descriptive statistics

### 2. **Data Cleaning**
   - Fill missing values using forward fill method
   - Remove redundant columns (Claim_ID)
   - Handle categorical variables using one-hot encoding

### 3. **Exploratory Data Analysis (EDA)**
   - Visualize claim status distribution
   - Analyze patient age demographics
   - Identify patterns and trends

### 4. **Feature Engineering**
   - Convert categorical variables to numerical format
   - Clean and standardize column names
   - Prepare feature matrix (X) and target variable (y)

### 5. **Model Development**
   - Split data into training (80%) and testing (20%) sets
   - Train Random Forest Classifier
   - Evaluate model performance

### 6. **Model Evaluation**
   - Calculate accuracy score
   - Generate classification report (precision, recall, F1-score)
   - Analyze feature importance

### 7. **Model Deployment**
   - Serialize and save model using joblib
   - Ready for production deployment

## 📈 Model Performance

The Random Forest Classifier provides:
- **Accuracy Score**: Model prediction accuracy on test set
- **Classification Metrics**: Precision, recall, and F1-score for each class
- **Feature Importance**: Identifies top factors influencing claim decisions

## 💡 Key Features

- Comprehensive data preprocessing pipeline
- Automatic handling of missing values
- Categorical variable encoding
- Feature importance analysis
- Model persistence for future predictions

## 🔧 Installation & Setup

1. Clone the repository:
```bash
git clone https://github.com/yourusername/healthcare-claims-prediction.git
cd healthcare-claims-prediction
```

2. Install required dependencies:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn joblib
```

3. Place your dataset:
```bash
# Copy healthcare_claims_large.csv to project directory
```

## ▶️ Usage

1. Open the Jupyter notebook:
```bash
jupyter notebook heart_deseas_project.ipynb
```

2. Execute cells sequentially to:
   - Load and explore data
   - Train the model
   - Generate predictions
   - View model performance metrics

3. Load pre-trained model:
```python
import joblib
model = joblib.load('model.pkl')
predictions = model.predict(new_data)
```

## 📊 Visualizations

The project includes:
- Claim status distribution chart
- Patient age histogram with KDE
- Feature importance bar chart
- Exploratory plots for data relationships

## 🎓 Learning Outcomes

This project demonstrates:
- End-to-end machine learning workflow
- Data preprocessing and cleaning techniques
- Exploratory data analysis methods
- Classification model development
- Model evaluation and interpretation
- Real-world healthcare analytics application

## 📝 Notes

- Ensure the dataset path is correctly specified in the notebook
- Missing values are handled using forward fill; consider alternative strategies if needed
- Feature scaling may improve model performance for certain algorithms
- Cross-validation can be added for more robust evaluation

## 🤝 Contributing

Contributions are welcome! Please feel free to:
- Submit issues for bugs or improvements
- Fork the repository and create pull requests
- Suggest enhancements to the analysis

## 📄 License

This project is open source and available under the MIT License.

## 👤 Author

Created for healthcare data analysis and machine learning applications.

## 📧 Contact & Support

For questions or suggestions, please open an issue in the repository.

---

**Last Updated**: March 2026
