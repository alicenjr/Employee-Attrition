# Employee Attrition Prediction 🚀

A machine learning project to predict employee attrition using Random Forest Classifier. This project analyzes HR data to identify patterns and factors that contribute to employee turnover.

## 📊 Project Overview

Employee attrition is a critical challenge for organizations. This project uses machine learning to predict whether an employee is likely to leave the company based on various factors such as satisfaction level, performance evaluation, number of projects, and more.

## 🎯 Features

- **Data Analysis**: Comprehensive exploratory data analysis of HR data
- **Feature Engineering**: One-hot encoding for categorical variables (Department, Salary)
- **Machine Learning Model**: Random Forest Classifier with optimized hyperparameters
- **Prediction**: Accurate prediction of employee attrition

## 📁 Dataset

The dataset (`HR_comma_sep.csv`) contains **14,999 employee records** with the following features:

| Feature | Description |
|---------|-------------|
| `satisfaction_level` | Employee satisfaction level (0-1) |
| `last_evaluation` | Last performance evaluation score (0-1) |
| `number_project` | Number of projects assigned |
| `average_montly_hours` | Average monthly working hours |
| `time_spend_company` | Years spent at the company |
| `Work_accident` | Whether had a work accident (0/1) |
| `left` | **Target Variable**: Whether employee left (0/1) |
| `promotion_last_5years` | Whether promoted in last 5 years (0/1) |
| `Department` | Department (sales, technical, support, IT, etc.) |
| `salary` | Salary level (low, medium, high) |

## 🛠️ Technologies Used

- **Python 3.x**
- **pandas**: Data manipulation and analysis
- **scikit-learn**: Machine learning model and evaluation
- **Jupyter Notebook**: Interactive development environment

## 📦 Installation

1. Clone the repository:
```bash
git clone https://github.com/alicenjr/Employee-Attrition.git
cd Employee-Attrition
```

2. Install required packages:
```bash
pip install pandas scikit-learn jupyter
```

3. Launch Jupyter Notebook:
```bash
jupyter notebook start.ipynb
```

## 🚀 Usage

1. **Load the data**:
   - The notebook loads the HR dataset from `HR_comma_sep.csv`

2. **Data Preprocessing**:
   - One-hot encoding for categorical variables (Department, Salary)
   - Feature-target split

3. **Model Training**:
   - Random Forest Classifier with 500 estimators
   - Train-test split (80-20)

4. **Model Evaluation**:
   - Accuracy score
   - Classification report
   - Confusion matrix

## 🧠 Model Details

### Random Forest Configuration
```python
RandomForestClassifier(
    n_estimators=500,
    criterion='gini',
    max_depth=2,
    min_samples_split=2,
    max_features='sqrt',
    random_state=45
)
```

### Model Performance
- **Training Set Size**: 11,999 samples
- **Test Set Size**: 3,000 samples
- **Features**: 20 (after encoding)

## 📈 Key Insights

The model analyzes various factors contributing to employee attrition:
- **Satisfaction Level**: Lower satisfaction increases attrition risk
- **Workload**: Number of projects and monthly hours
- **Career Development**: Promotion history and tenure
- **Departmental Trends**: Attrition patterns across departments
- **Compensation**: Impact of salary levels on retention

## 🔍 Model Workflow

```
Data Loading → Preprocessing → Feature Engineering → Train-Test Split → 
Model Training → Evaluation → Predictions
```

## 📊 Data Distribution

- **Total Employees**: 14,999
- **Attrition Rate**: ~24% (3,571 employees left)
- **Average Satisfaction**: 0.61
- **Average Projects**: 3.8
- **Average Monthly Hours**: 201

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/improvement`)
5. Open a Pull Request

## 📝 Future Enhancements

- [ ] Add data visualization dashboard
- [ ] Implement additional ML models (XGBoost, Neural Networks)
- [ ] Feature importance analysis
- [ ] Hyperparameter tuning with GridSearchCV
- [ ] Deploy model as a web application
- [ ] Add SHAP values for model interpretability

## 👨‍💻 Author

**Alice (Niraj)**
- GitHub: [@alicenjr](https://github.com/alicenjr)
- Email: hniraj51@gmail.com
- Bio: AI Engineer | Computer Vision, Automation & Microservices

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- HR dataset for employee attrition analysis
- scikit-learn documentation and community
- Open source contributors

---

⭐ If you find this project helpful, please consider giving it a star!

**Last Updated**: October 2025
