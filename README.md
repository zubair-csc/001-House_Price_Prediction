# 🏡 California House Price Prediction

## 📋 Project Overview

This project implements a comprehensive machine learning pipeline for predicting California house prices using the famous California Housing dataset. The project demonstrates advanced feature engineering techniques, multiple regression algorithms, and thorough model evaluation.

## 🎯 Objectives

- Predict median house values in California districts
- Explore and engineer features for better model performance
- Compare different regression algorithms
- Implement proper cross-validation and hyperparameter tuning
- Create visualizations for model interpretation

## 📊 Dataset Information

**Dataset**: California Housing Dataset (1990 Census)
- **Samples**: 20,640 districts
- **Features**: 8 numerical features
- **Target**: Median house value in hundreds of thousands of dollars

### Features:
- `longitude`: Longitude coordinate
- `latitude`: Latitude coordinate  
- `housing_median_age`: Median age of houses in district
- `total_rooms`: Total number of rooms in district
- `total_bedrooms`: Total number of bedrooms in district
- `population`: Total population in district
- `households`: Total number of households in district
- `median_income`: Median income of households in district

## 🔧 Technical Implementation

### Machine Learning Models:
- **Linear Regression**: Baseline model
- **Polynomial Regression**: Capturing non-linear relationships
- **Ridge Regression**: L2 regularization for overfitting prevention
- **Lasso Regression**: L1 regularization with feature selection
- **Random Forest**: Ensemble method for comparison

### Feature Engineering:
- **Derived Features**: 
  - `rooms_per_household`
  - `bedrooms_per_room`
  - `population_per_household`
- **Polynomial Features**: 2nd degree polynomial transformation
- **Feature Scaling**: StandardScaler for numerical features
- **Feature Selection**: SelectKBest and L1 regularization

### Model Evaluation:
- **Cross-Validation**: 5-fold CV for robust performance estimation
- **Metrics**: R², RMSE, MAE
- **Hyperparameter Tuning**: GridSearchCV for optimal parameters
- **Residual Analysis**: Checking model assumptions


## 🚀 Getting Started

### Prerequisites
```bash
Python 3.8+
Jupyter Notebook
```

### Installation
1. Clone the repository:
```bash
git clone https://github.com/zubair-csc/001-House_Price_Prediction.git
cd 001-House_Price_Prediction
```

2. Install required packages:
```bash
pip install -r requirements.txt
```

3. Launch Jupyter Notebook:
```bash
jupyter notebook House_Price_Prediction_with_Advanced_Feature_Engineering.ipynb
```

## 📋 Requirements

```
numpy>=1.21.0
pandas>=1.3.0
scikit-learn>=1.0.0
matplotlib>=3.4.0
seaborn>=0.11.0
jupyter>=1.0.0
```

## 📈 Results

### Model Performance:
| Model | R² Score | RMSE | MAE |
|-------|----------|------|-----|
| Linear Regression | 0.606 | 73.68 | 53.01 |
| Polynomial Regression | 0.678 | 66.51 | 48.92 |
| Ridge Regression | 0.664 | 68.09 | 49.56 |
| Lasso Regression | 0.664 | 68.09 | 49.56 |
| **Random Forest** | **0.806** | **51.64** | **33.31** |

### Key Insights:
- **Location matters**: Longitude and latitude are strong predictors
- **Income impact**: Median income shows strongest correlation with house prices
- **Feature engineering**: Derived features improved model performance by 12%
- **Non-linearity**: Polynomial features captured important non-linear relationships

## 📊 Visualizations

The notebook includes comprehensive visualizations:
- **Correlation Matrix**: Feature relationships
- **Actual vs Predicted**: Model accuracy visualization
- **Residual Plots**: Model assumption validation
- **Feature Importance**: Most influential features
- **Geographic Distribution**: Price patterns across California

## 🔍 Model Interpretation

### Feature Importance (Random Forest):
1. **Median Income** (38.2%)
2. **Longitude** (14.1%)
3. **Latitude** (11.3%)
4. **Housing Median Age** (8.9%)
5. **Population per Household** (7.8%)

## 📚 Learning Outcomes

This project demonstrates:
- **Data Preprocessing**: Handling missing values and outliers
- **Feature Engineering**: Creating meaningful derived features
- **Model Selection**: Comparing multiple algorithms systematically
- **Hyperparameter Tuning**: Optimizing model performance
- **Cross-Validation**: Ensuring robust model evaluation
- **Visualization**: Effective communication of results


## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request


## 👨‍💻 Author

**Zubair** - [GitHub](https://github.com/zubair-csc)

## 🙏 Acknowledgments

- California Housing Dataset from sklearn.datasets
- Scikit-learn documentation and community
- Jupyter Notebook for interactive development

## 📞 Contact

For questions or collaboration opportunities:
- GitHub: [@zubair-csc](https://github.com/zubair-csc)


