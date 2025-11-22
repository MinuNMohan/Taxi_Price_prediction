Taxi Trip Price Prediction Model

 Project Title
Taxi Trip Price Prediction using Machine Learning

## Objective
To develop an accurate machine learning model that predicts taxi trip prices based on various trip characteristics and  find the best performing modal
## Dataset Used
- **Dataset Name**: Taxi Trip Pricing Dataset
- **Source**:https://www.kaggle.com/datasets/denkuznetz/taxi-price-prediction/data
- **Dataset Characteristics**: 
  - 1,000 trip records
  - 11 features including trip distance, duration, time factors, traffic conditions, and pricing components
  - Target variable: Trip_Price (continuous)

## Models Used
The following machine learning regression models were implemented and compared:

1. **Random Forest Regressor** - Chosen for its ability to handle non-linear relationships, robustness to outliers, and high predictive accuracy through ensemble learning
2. **Decision Tree Regressor** - Selected as a baseline tree-based model for interpretability and fast training
3. **K-Neighbors Regressor** - Implemented to leverage similarity-based predictions and local patterns in the data
4. **Linear Regression** - Used as a simple baseline model to establish performance benchmarks
5. **Support Vector Regressor** - Applied to handle complex non-linear relationships using kernel methods


## Key Results
The models were evaluated using multiple regression metrics with the following results:

### Performance Metrics Comparison:
| Model | R² Score | MAE ($) | RMSE ($) |
|-------|----------|---------|----------|
| Random Forest | **0.9314** | **5.2739** | **7.5509** |
| Decision Tree | 0.8376 | 8.7195 | 11.6158 |
| K-Neighbors | 0.7822 | 10.7921 | 13.4503 |
| Linear Regression | 0.7702 | 9.8887 | 13.8177 |
| Support Vector Machine | 0.5326 | 10.8020 | 19.7045 |

### Best Performing Model:
**Random Forest Regressor** achieved the highest performance across all evaluation metrics:
- **R² Score**: 0.9314 (93.14% of variance explained)
- **Mean Absolute Error (MAE)**: $5.27
- **Root Mean Squared Error (RMSE)**: $7.55

### Outcome Summary:
The Random Forest model demonstrated exceptional predictive capability, accurately estimating taxi trip prices with an average error of approximately $5.27. The model successfully captured the complex relationships between trip characteristics and pricing, making it suitable for real-world deployment in taxi fare estimation systems. The high R² score of 0.9314 indicates that the model explains over 93% of the variance in taxi prices, providing reliable predictions for practical applications.
