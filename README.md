# Customer Churn Analysis 📉

This project analyzes customer churn using visualization and predictive modeling. We explore relationships in the data and predict churn using regression and classification techniques.

---

## 📊 Data Visualization

### 1. Internet Service Distribution
- Bar plot of `InternetService` categories.

![Internet Service Distribution](images/Internet%20Service%20Distribution.png)


### 2. Tenure Distribution
- Histogram showing distribution of `tenure`.

![Tenure Histogram](images/Tenure%20Histogram.png)

### 3. Monthly Charges vs Tenure
- Scatter plot showing relationship between `MonthlyCharges` and `tenure`.

![Monthly Charges vs Tenure](images/Monthly%20Charges%20vs%20Tenure.png)

### 4. Box Plot: Tenure by Contract Type
- Shows variation of `tenure` across different `Contract` types.

![Tenure Boxplot by Contract](images/Tenure%20Boxplot%20by%20Contract.png)

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
- 📊 **Confusion Matrix**:`[[1797    0]
                            [ 669    0]]`



---

### b. Multiple Logistic Regression
- **Target**: `Churn`  
- **Features**: `tenure`, `MonthlyCharges`  
- **Train/Test Split**: 80:20

**Model Evaluation:**
- ✅ **Accuracy Score**: `79.85%`
- 📊 **Confusion Matrix**:`[[944  92]
                            [193 180]]`



---

## 🌳 Decision Tree

- **Target**: `Churn`
- **Feature**: `tenure`
- **Train/Test Split**: 80:20

**Model Evaluation:**
- ✅ **Accuracy Score**: `73.19%`
- 📊 **Confusion Matrix**:`[[951  85]
                            [257 116]]`



---

## 🌲 Random Forest

- **Target**: `Churn`
- **Features**: `tenure`, `MonthlyCharges`
- **Train/Test Split**: 70:30

**Model Evaluation:**
- ✅ **Accuracy Score**: `79.63%`
- 📊 **Confusion Matrix**:`[[1341  198]
                            [ 308  266]]`




---

## 🧪 Requirements

```bash
pip install pandas matplotlib seaborn scikit-learn


