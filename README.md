# 🔮 Future Self Predictor (FSP)

This project predicts a person’s **future outcome score** and categorizes it into **Low, Medium, or High** using a machine learning regression model.

The project is implemented using **Python** and trained on a structured dataset with numerical features.

---

## 📌 Project Overview
The **Future Self Predictor** uses a **Random Forest Regressor** to estimate a future score based on multiple input features.  
The predicted score is then converted into a meaningful category:
- **Low**
- **Medium**
- **High**

The trained model is saved using **Pickle** for future reuse.

---

## 🧠 Problem Statement
To build a machine learning model that:
1. Predicts a numerical **future score**
2. Converts the score into a categorical outcome (Low / Medium / High)
3. Saves and reloads the trained model for future predictions

---

## ⚙️ Technologies & Libraries Used
- Python
- Google Colab
- Pandas
- NumPy
- Scikit-learn
- RandomForestRegressor
- StandardScaler
- Pickle

---

## 🗂 Dataset
- Dataset used: `future_self_dataset_100k.csv`
- Contains multiple numerical input features
- Target column: `output_score`

### Category Mapping Logic
- `≤ 33` → Low  
- `34 – 66` → Medium  
- `> 66` → High  

---

## 🔄 Project Workflow
1. Import required libraries  
2. Load dataset and remove null values  
3. Convert numerical output into categorical labels  
4. Split data into training and testing sets  
5. Apply feature scaling using StandardScaler  
6. Train model using RandomForestRegressor  
7. Evaluate model using Mean Squared Error (MSE)  
8. Save trained model using Pickle  
9. Load model and predict on new input data  

---

## 📈 Model Performance
- Algorithm Used: Random Forest Regressor  
- Evaluation Metric: Mean Squared Error (MSE)  
- Achieved MSE: ~27  

---

## 🧪 Sample Prediction

Input Features:
[52, 70, 35, 10, 9, 9, 95]
Output:
Predicted Score: 53.88
