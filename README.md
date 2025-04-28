# Housing Price Prediction using Linear Regression

## Project Overview
This project predicts housing prices using **Simple and Multiple Linear Regression**. The dataset includes features like area, bedrooms, bathrooms, and furnishing status.

## Dataset
- **Source**: [Housing.csv](data/Housing.csv)
- **Features**: `area`, `bedrooms`, `bathrooms`, `stories`, `mainroad`, `guestroom`, `basement`, `hotwaterheating`, `airconditioning`, `parking`, `prefarea`, `furnishingstatus`
- **Target**: `price`

## Steps
1. **Data Preprocessing**:  
   - Converted categorical variables (`yes/no`) to binary (`1/0`).  
   - Applied one-hot encoding to `furnishingstatus`.  

2. **Model Training**:  
   - Used `sklearn.linear_model.LinearRegression`.  
   - Split data into 80% train, 20% test.  

3. **Evaluation Metrics**:  
   - **MAE**: 700,000  
   - **MSE**: 8.2e+11  
   - **R²**: 0.65  

4. **Results**:  
   - The model explains **65% of price variance**.  
   - Key predictors: `area`, `bathrooms`, `airconditioning`.  

## How to Run
1. Install dependencies:  
   ```bash
   pip install -r requirements.txt
