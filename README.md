Here's your **README** file with emojis to make it more engaging! 🚀🏡💡  

---

# 🏠 Housing Price Prediction using XGBoost Regressor 🚀  

This project demonstrates the prediction of **housing prices** in **California** 🏡 using the **California Housing dataset** 📊 and the **XGBoost Regressor** model 🤖.  

## 📌 Table of Contents  

- 🔍 [Project Overview](#-project-overview)  
- 📂 [Dataset Description](#-dataset-description)  
- 📦 [Dependencies](#-dependencies)  
- 🛠️ [How to Run the Code](#-how-to-run-the-code)  
- 📊 [Model Evaluation](#-model-evaluation)  
- 📈 [Results](#-results)  
- 🎨 [Visualizations](#-visualizations)  
- 📜 [License](#-license)  

---

## 🔍 Project Overview  

The goal of this project is to **predict median house values** in California districts based on features like **income levels**, **house age**, and **geographical location**.  

The model used for prediction is **XGBoost Regressor** 🌲, a powerful decision-tree-based ensemble model that is highly efficient for regression tasks.  

---

## 📂 Dataset Description  

This project uses the **California Housing dataset** 🗂️ from **scikit-learn**, which includes:  

🔹 **MedInc**: Median income of the block group 🏦  
🔹 **HouseAge**: Median house age of the block group 🏘️  
🔹 **AveRooms**: Average number of rooms per household 🏡  
🔹 **AveBedrms**: Average number of bedrooms per household 🛏️  
🔹 **Population**: Block group population 👥  
🔹 **AveOccup**: Average household size 👨‍👩‍👧‍👦  
🔹 **Latitude**: Geographic latitude 🌍  
🔹 **Longitude**: Geographic longitude 🌍  
🔹 **Price (Target Variable)**: Median house value 💰  

📊 **Dataset Info:**  
✔️ **Instances**: 20,640 🏠  
✔️ **Features**: 8 predictive features 📊  

---

## 📦 Dependencies  

The following **Python libraries** are required to run this project:  

📌 `numpy` 📌 `pandas` 📌 `matplotlib` 📌 `seaborn`  
📌 `scikit-learn` 📌 `xgboost`  

📌 Install dependencies using:  
```bash
pip install numpy pandas matplotlib seaborn scikit-learn xgboost
```

---

## 🛠️ How to Run the Code  

1️⃣ **Clone the Repository** 🛠️  
```bash
git clone https://github.com/your-username/Housing-Price_prediction.git
cd Housing-Price_prediction
```

2️⃣ **Run the Script** 🚀  
```bash
python housing_price_prediction.py
```

📌 This will:  
✅ Load and preprocess the dataset 📊  
✅ Train the **XGBoost Regressor** model 🌲  
✅ Evaluate model performance 📉  
✅ Generate **visualizations** (e.g., heatmaps, scatter plots) 📊  

---

## 📊 Model Evaluation  

After training, the model is **evaluated** using:  

✔️ **R-squared (R²)** - Measures how well the model explains the variance in house prices  
✔️ **Mean Absolute Error (MAE)** - Measures the average prediction error  

📉 **Training Data Evaluation**:  
✅ **R² Score**: **0.9446** 🔥  
✅ **MAE**: **0.1926** 📉  

📉 **Testing Data Evaluation**:  
✅ **R² Score**: **0.8301** 🎯  
✅ **MAE**: **0.3096** 📉  

---

## 📈 Results  

📌 The **XGBoost Regressor model** performs well, achieving an **R² of 0.9446** on training data and **0.8301 on testing data**, indicating **strong predictive power**! 🚀  

📌 Slight **overfitting** is observed, but the model **generalizes well** to unseen data.  

---

## 🎨 Visualizations  

🔹 **Correlation Heatmap** 📊 - Displays feature relationships  
🔹 **Actual vs Predicted Price Scatter Plot** 📈 - Shows model accuracy  

---

## 📜 License  

This project is licensed under the **MIT License** 📄 - see the **LICENSE** file for details.  

---

💡 **Notes:**  
📌 Ensure compatibility by updating XGBoost and Scikit-learn:  
```bash
pip install --upgrade xgboost scikit-learn
```  
📌 The dataset is publicly available via **scikit-learn** 🎓.  

---

🚀 Happy Coding! 🏡💻✨  
