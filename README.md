# Housing Price Prediction using XGBoost Regressor

This project demonstrates the prediction of housing prices in California using the California Housing dataset and the XGBoost Regressor model.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Dataset Description](#dataset-description)
3. [Dependencies](#dependencies)
4. [How to Run the Code](#how-to-run-the-code)
5. [Model Evaluation](#model-evaluation)
6. [Results](#results)
7. [Visualizations](#visualizations)
8. [License](#license)

---

## Project Overview

The goal of this project is to predict the median house value in California districts based on several features such as median income, house age, average number of rooms, and geographical location. The model used for prediction is the **XGBoost Regressor**, a decision-tree-based ensemble model that is highly efficient for regression tasks.

---

## Dataset Description

This project uses the **California Housing dataset**, which is available through the `scikit-learn` library. It contains the following features:

- **MedInc**: Median income in the block group.
- **HouseAge**: Median house age in the block group.
- **AveRooms**: Average number of rooms per household.
- **AveBedrms**: Average number of bedrooms per household.
- **Population**: Block group population.
- **AveOccup**: Average number of household members.
- **Latitude**: Latitude of the block group.
- **Longitude**: Longitude of the block group.
- **Price** (Target Variable): The median house value in California districts (target variable, expressed in hundreds of thousands of dollars).

### Dataset Info:
- **Number of Instances**: 20,640
- **Number of Attributes**: 8 features (predictive) and 1 target variable (price)

---

## Dependencies

The following Python libraries are required to run this project:

- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `xgboost`

You can install these dependencies using pip:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn xgboost
```

---

## How to Run the Code

1. **Clone the Repository**:

   First, clone this repository to your local machine:

   ```bash
   git clone https://github.com/your-username/Housing-Price_prediction.git
   cd Housing-Price_prediction
   ```

2. **Run the Script**:

   Ensure you have all dependencies installed (use the command above), then simply run the script:

   ```bash
   python housing_price_prediction.py
   ```

   This will:
   - Load and preprocess the dataset
   - Train the XGBoost Regressor model
   - Evaluate the model using R-squared and Mean Absolute Error
   - Generate visualizations (like correlation heatmap and actual vs predicted price scatter plot)

---

## Model Evaluation

Once the model is trained, it is evaluated on both the training and testing data. The following metrics are calculated:

1. **R-squared**: Measures the proportion of the variance in the target variable (house price) that is predictable from the features.
2. **Mean Absolute Error (MAE)**: Measures the average magnitude of the errors in predictions, without considering their direction.

### Evaluation on Training Data:
- **R-squared**: 0.9446
- **Mean Absolute Error (MAE)**: 0.1926

### Evaluation on Testing Data:
- **R-squared**: 0.8301
- **Mean Absolute Error (MAE)**: 0.3096

---

## Results

The XGBoost Regressor model performs well on the training data, achieving a high R-squared value of approximately **0.9446**, indicating that the model explains most of the variance in house prices. However, the model's performance drops slightly on the testing data with an R-squared of **0.8301**, indicating some overfitting, but the model still generalizes well.

---

## Visualizations

The following visualizations are generated:

1. **Correlation Heatmap**: Shows the correlation between different features and the target variable (price).
2. **Actual vs Predicted Price Scatter Plot**: Visualizes the accuracy of the model's predictions by plotting actual house prices against predicted house prices on the training data.

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

### Notes:
1. Ensure you have the correct versions of `XGBoost` and `scikit-learn` to avoid compatibility issues. You can update them using `pip install --upgrade xgboost scikit-learn`.
2. This project uses the California Housing dataset available through `scikit-learn`.

---
