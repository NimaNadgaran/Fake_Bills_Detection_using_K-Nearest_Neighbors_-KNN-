# 🧠 Fake Bills Detection using K-Nearest Neighbors (KNN)

This project demonstrates how to use the **K-Nearest Neighbors (KNN)** algorithm to classify **genuine vs. fake bills** based on physical and geometric measurements.

It includes **data preprocessing**, **encoding**, **scaling**, **model training**, and **visual evaluation** using a confusion matrix and classification report.

---

## 📁 Dataset

**File:** `fake_bills.csv`

The dataset contains several geometric features of banknotes.  
Each row represents one bill, and the goal is to predict whether it is **genuine** or **fake**.

| Column Name   | Description |
|----------------|-------------|
| `is_genuine`   | Target label: `True` for genuine, `False` for fake |
| `diagonal`     | Length of the bill’s diagonal |
| `height_left`  | Height measured from the left side |
| `height_right` | Height measured from the right side |
| `margin_low`   | Lower margin of the bill |
| `margin_up`    | Upper margin of the bill |
| `length`       | Length of the bill |

---

## ⚙️ Steps Performed

### 1. **Data Loading**
Load and parse the CSV file using a semicolon (`;`) separator:

### 2. Data Cleaning

Fill missing values in the margin_low column using the median.

### 3. Label Encoding

Convert the target column is_genuine from True/False to numeric (1/0).

### 4. Feature Scaling

Standardize all numeric features using StandardScaler.

### 5. Train/Test Split

Split the data into 80% training and 20% testing sets.

### 6. KNN Model Training

Train a KNN model with k = 5.

### 7. Model Evaluation

Check training and testing accuracy.

### 8. Visualization
🔹 Confusion Matrix


## Model Accuracy:
```
Training accuracy: 0.9933333333333333
Testing accuracy: 0.99

```

Also the name of the file of the code comes from the brand of my friend's bag.

