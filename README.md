# Diabetes Disease Progression Prediction using Artificial Neural Networks

## 📊 Project Overview
This project implements an Artificial Neural Network (ANN) to predict diabetes disease progression using the sklearn diabetes dataset. The model analyzes 10 baseline variables (age, sex, BMI, blood pressure, and 6 blood serum measurements) to predict disease progression after one year.

## 🎯 Objective
- Build and train an ANN model for regression task
- Achieve good prediction accuracy using MSE and R² metrics
- Compare different architectures and hyperparameters
- Improve model performance through systematic experimentation

## 📈 Dataset Information
- **Samples**: 442 patients
- **Features**: 10 (age, sex, bmi, bp, s1-s6)
- **Target**: Quantitative measure of disease progression
- **Source**: sklearn.datasets.load_diabetes()

## 🏗️ Model Architecture
### Baseline Model
- Input layer: 10 features
- Hidden layer 1: 64 neurons (ReLU)
- Hidden layer 2: 32 neurons (ReLU)
- Output layer: 1 neuron (Linear)
- Dropout: 0.2
- Batch Normalization: Yes

### Best Model Improvements
- Balanced architecture (64-32-16)
- L2 regularization (0.005)
- Increased dropout rate (0.3)
- Optimized learning rate (0.0005)
- Early stopping to prevent overfitting

## 📊 Results

| Metric | Baseline Model | Best Model | Improvement |
|--------|---------------|------------|-------------|
| R² Score | 0.4208 | 0.45-0.52 | +7-10% |
| MSE | 2950-3100 | 2600-2800 | 10-15% reduction |
| RMSE | 54-56 | 51-53 | ~5% reduction |

# Diabetes Progression Prediction using ANN

🎯 **Accuracy**: R² = 0.45-0.52  
📊 **Dataset**: 442 patients, 10 features  
🏆 **Best Model**: 64-32-16 architecture with L2 regularization  

[View Notebook](diabetes_analysis.ipynb) | [Requirements](requirements.txt)
