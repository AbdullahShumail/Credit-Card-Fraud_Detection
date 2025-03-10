## 🚀 Credit Card Fraud Detection System

### 🌟 Overview
The **Credit Card Fraud Detection System** is a powerful machine learning project designed to identify **fraudulent credit card transactions** 💳. It leverages **Logistic Regression** to detect suspicious activities, helping prevent financial loss by catching fraud in action! 🔒

### 📊 Dataset
We use a dataset containing **284,807 transactions** with 30 feature columns (`V1` to `V28`, `Time`, and `Amount`) and a target column (`Class`).
- **Class 1:** Fraudulent transaction 🔴
- **Class 0:** Legitimate transaction ✅

⚠️ **Note:** The dataset is **highly imbalanced**, with only **473 fraud cases** (about **0.17%** of all transactions).

### ⚙️ Steps Involved
1. **🔍 Data Preprocessing:**
   - Cleaned the data by removing duplicates and handling missing values.
   - Visualized class distribution and feature correlations using **pie charts** and **heatmaps**.

2. **📈 Feature Selection:**
   - Utilized all 30 features for model training.

3. **🤖 Model Training:**
   - Split the data into **training (75%)** and **testing (25%)** sets.
   - Trained a **Logistic Regression model** for binary classification.

4. **📊 Model Evaluation:**
   - **Training Accuracy:** 99.89% ✅
   - **Testing Accuracy:** 99.90% ✅
   - Assessed performance using **confusion matrices**, **precision**, **recall**, and **F1-scores**.

### 📈 Evaluation Metrics
- **🎯 Precision:** How many of the predicted fraud cases were actually fraud.
- **⚡ Recall:** How many real fraud cases were correctly identified.
- **📊 F1-Score:** A balance between precision and recall.
- **🟢 Confusion Matrix:** Highlights **true positives**, **false positives**, **true negatives**, and **false negatives**.

### 🏆 Results
Despite the high accuracy, the model faced challenges due to data imbalance. Key metrics:
- **🔴 Precision for fraud detection:** 71% (testing data)
- **⚡ Recall for fraud detection:** 68% (testing data)

### 📊 Visualization
- **🥧 Pie Chart:** Class distribution (fraud vs. not fraud).
- **🔥 Heatmap:** Feature correlations.

### 📦 Saving and Loading the Model with Joblib
Want to save your trained model and reuse it anytime? Here’s how you can do it with **joblib**:

**1. Install joblib:**
```bash
pip install joblib
```

**2. Import joblib:**
```python
import joblib
```

**3. Save the trained model:**
```python
joblib.dump(logit, 'credit_card_fraud_model.pkl')
```

**4. Load the model later:**
```python
loaded_model = joblib.load('credit_card_fraud_model.pkl')
```

**5. Make predictions with the loaded model:**
```python
predictions = loaded_model.predict(x_test)
print(predictions)
```

### 📥 Download the Model to Your PC
Once you’ve saved the `.pkl` file, you can download it to your computer.

**In Jupyter Notebook:**
```python
from IPython.display import FileLink
FileLink('credit_card_fraud_model.pkl')
```

**In Google Colab:**
```python
from google.colab import files
files.download('credit_card_fraud_model.pkl')
```

Click the link generated to download the model directly to your PC! 💾

### 🌟 Conclusion
The **Credit Card Fraud Detection System** efficiently identifies fraudulent transactions using **Logistic Regression** 🔥. While the model performs well, future enhancements could include:
- 🌲 **Exploring advanced models** like **Random Forest** or **Neural Networks**.
- ⚖️ **Handling data imbalance** with techniques like **SMOTE**.
- ⏳ **Implementing real-time fraud detection**.

### 🏃‍♀️ How to Run
1. **Install dependencies:**
```bash
pip install pandas numpy seaborn matplotlib scikit-learn
```
2. **Load and clean the dataset.**
3. **Train the Logistic Regression model.**
4. **Evaluate the model’s performance** using confusion matrices and classification reports.
5. **Save and download the trained model** using joblib.

### 👨‍💻 Author
- **Abdullah Shumail** ✨

---

Let’s fight fraud with AI! 🚀💳

