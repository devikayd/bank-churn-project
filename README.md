# Bank Customer Churn Prediction 📊

A machine learning project to predict customer churn and segment customers for targeted retention strategies.

## Project Overview 📝

Customer churn is a critical problem for banks. Acquiring new customers costs significantly more than retaining existing ones. This project aims to:

1. Identify which customers are likely to churn
2. Understanding the key factors driving churn
3. Segment customers for targeted retention campaigns
4. Build predictive models with explainable insights

## Dataset

- **Source:** Kaggle - Bank Customer Churn Dataset
  🔗 https://www.kaggle.com/datasets/radheshyamkollipara/bank-customer-churn?select=Customer-Churn-Records.csv
- **Size:** 10,000 customers
- **Features:** 14 columns including demographics, account information, and activity status
- **Target:** Exited (1 = Churned, 0 = Stayed)

## Key Findings from EDA

| Factor | Insight |
|--------|---------|
| Geography | Germany has 32.4% churn vs ~16% for France/Spain |
| Age | Older customers churn more (avg 45 vs 36) |
| Products | 2 products = 7.6% churn, 3+ products = 80%+ churn |
| Activity | Inactive members: 26.9% churn vs Active: 14.3% |
| Gender | Female: 25.1% churn vs Male: 16.5% |

## Project Structure
```
bank-churn-project/
├── data/
│   ├── raw/                 # Original dataset
│   └── processed/           # Cleaned data
├── notebooks/
│   ├── customer-churn.ipynb
│   ├── exploratory_data-analysis.ipynb
│   ├── data_preprocessing.ipynb
│   ├── customer_segmentation.ipynb
│   └── churn_prediction.ipynb
├── outputs/
│   ├── figures/             # Visualizations
│   └── models/              # Saved models
├── src/                     # Python scripts
├── requirements.txt
└── README.md
```

## Tech Stack

- **Python 3.x**
- **Data Manipulation:** Pandas, NumPy
- **Visualization:** Matplotlib, Seaborn, Plotly
- **Machine Learning:** Scikit-learn, XGBoost
- **Explainability:** SHAP
- **Imbalanced Data:** imbalanced-learn (SMOTE)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/devikayd/bank-churn-project.git
cd bank-churn-project
```

2. Create virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

## Results

- Model Performance (AUC-ROC, F1-Score)
- Feature Importance
- Customer Segments

## Future Improvements

- Deploy model as API
- Create interactive dashboard
- Add real-time prediction capability

## Author

Your Name

- LinkedIn: 
- Email: your.email@example.com

## License

This project is open source and available under the MIT License.