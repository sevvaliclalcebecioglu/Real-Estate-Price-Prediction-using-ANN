# Real Estate Price Prediction using ANN

This project aims to predict real estate prices in Taiwan using historical data and several features with an **Artificial Neural Network (ANN)**.

## Technologies Used
- Python 3.x
- Pandas, NumPy
- Scikit-learn
- PyTorch (ANN)
- Matplotlib, Seaborn (for visualization)
- Streamlit (optional for web application)

## Dataset
| Column | Description | Type |
|--------|-------------|------|
| Transaction date | Date of transaction | object |
| House age | Age of the house (years) | float64 |
| Distance to nearest MRT station | Distance to the nearest metro station | float64 |
| Number of convenience stores | Number of nearby convenience stores | int64 |
| Latitude | Latitude | float64 |
| Longitude | Longitude | float64 |
| House price per unit area | Target variable: price per square meter | float64 |

## Data Preprocessing
- Missing values removed or imputed
- Numerical features normalized
- Train-test split: 80%-20%

## Model and Training
- ANN: 3 hidden layers (64-32-16)
- Activation: ReLU
- Optimizer: SGD, learning rate 0.01
- Epochs: 130 with Early Stopping
- Loss: MSE (Mean Squared Error)

## Performance Results
| Model | R² | RMSE | MAE |
|-------|----|------|-----|
| ANN (DL) | 0.16 | 11.85 | 9.95 |

- Compared with other regression models: KNeighbors, Ridge, Gradient Boosting, etc.  
- Results show limited performance; the dataset is small and some features may not be sufficient for accurate predictions.

## Lessons Learned
- Regression predictions with ANN
- Data normalization and feature engineering
- Model evaluation using R², RMSE, MAE
- Early stopping and model saving

## Future Work
- Use larger and more diverse datasets
- Hyperparameter optimization
- Experiment with different model architectures
