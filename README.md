# Student Performance Prediction

This project aims to predict students' math scores using machine learning models. The dataset includes demographic, parental, and educational background features. The project uses several regression models to evaluate performance and find the best-performing algorithm.

## Table of Contents
1. [Overview](#overview)
2. [Dataset](#dataset)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Features](#features)
6. [Model Performance](#model-performance)
7. [Technologies Used](#technologies-used)
8. [License](#license)

---

## Overview
The project involves:
- Preprocessing student demographic and test data.
- Training multiple regression models to predict math scores.
- Evaluating models based on R², RMSE, and MAE.

---

## Dataset
The dataset used for this project contains the following features:
- `gender`: Gender of the student.
- `race_ethnicity`: Ethnic group of the student.
- `parental_level_of_education`: Highest level of education completed by parents.
- `lunch`: Type of lunch the student receives (standard or free/reduced).
- `test_preparation_course`: Whether the student completed the test preparation course.
- `math_score`: Target variable for prediction.
- `reading_score` and `writing_score`: Additional test scores.

---

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/student-performance-prediction.git
   cd student-performance-prediction
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

---

## Usage
1. Place the dataset in the `data/` folder.
2. Run the preprocessing script:
   ```bash
   python preprocessing.py
   ```
3. Train the models:
   ```bash
   python model_training.py
   ```
4. View performance metrics in the console or generated reports.

---

## Features
- **Data Preprocessing**: Categorical encoding, feature scaling, and train-test splitting.
- **Model Training**: Implements multiple regression models including Linear Regression, Decision Tree, Random Forest, XGBoost, CatBoost, and AdaBoost.
- **Performance Metrics**: Includes R², RMSE, and MAE for training and test sets.

---

## Model Performance
The following table summarizes model performance (Test Set):

| Model                     | RMSE   | MAE   | R²    |
|---------------------------|--------|-------|-------|
| Linear Regression         | 5.39   | 4.21  | 0.880 |
| Lasso                     | 6.52   | 5.16  | 0.825 |
| Ridge                     | 5.39   | 4.21  | 0.881 |
| K-Neighbors Regressor     | 7.25   | 5.62  | 0.784 |
| Decision Tree             | 8.08   | 6.43  | 0.732 |
| Random Forest Regressor   | 5.96   | 4.60  | 0.854 |
| XGBRegressor              | 6.47   | 5.06  | 0.828 |
| CatBoosting Regressor     | 6.01   | 4.61  | 0.852 |
| AdaBoost Regressor        | 5.80   | 4.77  | 0.851 |

---

## Technologies Used
- Python
- Scikit-learn
- XGBoost
- CatBoost
- NumPy
- Pandas
- Matplotlib
- Seaborn

---

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
```

Let me know if you need any changes!
