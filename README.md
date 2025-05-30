# Customer Churn Analysis 📉

This project analyzes customer churn using visualization and predictive modeling. We explore relationships in the data and predict churn using regression and classification techniques.

---

## 📊 Data Visualization

### 1. Internet Service Distribution
- Bar plot of `InternetService` categories.

![Internet Service Distribution](images/internet_service_barplot.png)

### 2. Tenure Distribution
- Histogram showing distribution of `tenure`.

![Tenure Histogram](images/tenure_histogram.png)

### 3. Monthly Charges vs Tenure
- Scatter plot showing relationship between `MonthlyCharges` and `tenure`.

![Monthly Charges vs Tenure](images/monthlycharges_tenure_scatter.png)

### 4. Box Plot: Tenure by Contract Type
- Shows variation of `tenure` across different `Contract` types.

![Tenure Boxplot by Contract](images/tenure_contract_boxplot.png)

---

## 📈 Linear Regression

- **Target**: `MonthlyCharges`
- **Feature**: `tenure`
- **Train/Test Split**: 70:30

**Model Evaluation:**
- 🔢 **Root Mean Squared Error (RMSE)**: `29.36`

---

## 🔐 Logistic Regression

### a. Simple Logistic Regression
- **Target**: `Churn`  
- **Feature**: `MonthlyCharges`  
- **Train/Test Split**: 65:35

**Model Evaluation:**
- ✅ **Accuracy Score**: `79.76%`
- 📊 **Confusion Matrix**:




Confusion Matrix (Simple Model):
[[1797    0]
 [ 669    0]]
Accuracy Score (Simple Model): 0.7287104622871047
Confusion Matrix (Multiple Model):
[[944  92]
 [193 180]]
Accuracy Score (Multiple Model): 0.7977288857345636



---

### b. Multiple Logistic Regression
- **Target**: `Churn`  
- **Features**: `tenure`, `MonthlyCharges`  
- **Train/Test Split**: 80:20

**Model Evaluation:**
- ✅ **Accuracy Score**: `79.85%`
- 📊 **Confusion Matrix**:


---

## 🌳 Decision Tree

- **Target**: `Churn`
- **Feature**: `tenure`
- **Train/Test Split**: 80:20

**Model Evaluation:**
- ✅ **Accuracy Score**: `73.19%`
- 📊 **Confusion Matrix**:



---

## 🌲 Random Forest

- **Target**: `Churn`
- **Features**: `tenure`, `MonthlyCharges`
- **Train/Test Split**: 70:30

**Model Evaluation:**
- ✅ **Accuracy Score**: `79.63%`
- 📊 **Confusion Matrix**:




---

## 🧪 Requirements

```bash
pip install pandas matplotlib seaborn scikit-learn


