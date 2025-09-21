# Car-Price-Prediction-Machine-Learning-Project

This project focuses on predicting the **selling price of used cars** using machine learning techniques. The goal is to build a regression model that can accurately estimate a car's price based on various features such as its brand, year, mileage, and other specifications.

---

## 📂 Dataset
- **File Name:** `car data.csv`  
- **Entries:** 301  
- **Columns:** 9  

### Features:
- `Car_Name`
- `Year`
- `Selling_Price` *(Target Variable)*
- `Present_Price`
- `Kms_Driven`
- `Fuel_Type`
- `Seller_Type`
- `Transmission`
- `Owner`

✅ The dataset has **no missing values**, which simplifies preprocessing.

---

## ⚙️ Methodology

The project follows a standard **machine learning workflow**:

1. **📊 Data Preprocessing & Analysis**  
   - Load dataset using Pandas.  
   - Perform exploratory data analysis.  
   - Encode categorical variables (`Fuel_Type`, `Seller_Type`, `Transmission`) into numerical form.  

2. **✂️ Feature & Target Separation**  
   - Features: All columns except `Selling_Price`.  
   - Target: `Selling_Price`.  

3. **🔀 Train-Test Split**  
   - Use `train_test_split` from Scikit-learn to split the dataset into **training** and **testing** sets.  

4. **🤖 Model Training**  
   Two regression models are applied:
   - **Linear Regression** → Establishes a linear relationship between features and target.  
   - **Lasso Regression** → Linear regression with L1 regularization (helps feature selection & reduces overfitting).  

5. **📈 Model Evaluation**  
   - Evaluate using **R-squared error metric** to determine model performance.  
