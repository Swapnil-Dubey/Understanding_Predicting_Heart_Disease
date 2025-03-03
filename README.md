# Heart Disease Inference and Prediction System 

![R](https://img.shields.io/badge/R-4.3.2-blue?logo=r) ![License](https://img.shields.io/badge/License-MIT-green)

Clinical decision support system analyzing 13 medical parameters to predict cardiovascular risk with 79.8% accuracy. Identifies key risk factors through logistic regression and regularization techniques.

## Dataset Overview 📊
**Source**: UCI Machine Learning Repository (Cleveland subset)  
**Samples**: 303 patient records  
**Features**: 13 clinical parameters + 1 outcome variable

| Parameter       | Description                                  | Type        |
|-----------------|---------------------------------------------|-------------|
| `age`           | Patient age in years                        | Continuous  |
| `sex`           | Biological sex (0=Female, 1=Male)           | Categorical |
| `cp`            | Chest pain type (1-4)                       | Categorical |
| `thalach`       | Maximum heart rate achieved                 | Continuous  |
| `exang`         | Exercise-induced angina (0/1)               | Categorical |
| `thal`          | Thalassemia status (3/6/7)                  | Categorical |
| *[Full list in report]* | | |

## Key Findings 🚨
**Top Risk Multipliers**:
- ⚠️ Male patients: 3.69× higher risk
- ⚠️ Asymptomatic chest pain: 5.4× higher risk  
- ⚠️ Reversible thalassemia defect: 8.7× higher risk

**Model Performance**:
| Model  | Accuracy | Precision | Recall | ROC-AUC |
|--------|----------|-----------|--------|---------|
| OLS    | 79.8%    | 82.8%     | 80.3%  | 0.84    |
| Lasso  | 79.8%    | 84.4%     | 79.4%  | 0.83    |

## Setup ⚙️
install.packages(c("dplyr", "glmnet", "rsample", "GGally"))
