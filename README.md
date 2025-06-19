## 🏡 House Prices: Exploratory Data Analysis (EDA)

This project performs a thorough Exploratory Data Analysis (EDA) on the popular **House Prices - Advanced Regression Techniques** dataset from Kaggle. The goal is to understand the underlying data, visualize patterns, detect outliers, handle missing values, and explore relationships that can influence house sale prices.

---

### 📁 Dataset

* **Source:** [Kaggle - House Prices Dataset](https://www.kaggle.com/c/house-prices-advanced-regression-techniques)
* **File Used:** `train.csv`
* **Records:** 1,460 houses
* **Features:** 80 explanatory variables (numerical, categorical) + target (`SalePrice`)

---

### 🔍 EDA Workflow

The analysis follows a systematic EDA process:

#### 1. 📥 Data Loading & Structure Check

* Loaded CSV using `pandas`
* Previewed data using `.head()`, `.info()`, `.describe()`

#### 2. 🏷️ Data Type Inspection

* Identified numeric vs categorical columns
* Checked for potential incorrect data types

#### 3. ⚠️ Missing Values Analysis

* Tabulated missing counts
* Visualized using a heatmap (`sns.heatmap`)

#### 4. 📊 Univariate Analysis

* **Histograms & KDE plots** for numerical columns
* Identified skewness and unusual distributions

#### 5. 📈 Outlier Detection

* Used **IQR method** to detect outliers in `SalePrice`
* Visualized outliers using **boxplots** and **log-transformed scatterplots**

#### 6. 🔗 Correlation Analysis

* Generated **correlation heatmap**
* Identified top features correlated with `SalePrice`

#### 7. 🧠 Categorical Feature Exploration

* Countplots for category distributions
* Boxplots & violin plots for relationships with `SalePrice`

---

### 📷 Sample Visualizations

* Heatmaps of missing values and correlations
* Histograms for numeric features
* Log-scale scatter plot (`GrLivArea` vs `SalePrice`)
* Boxplots/Violin plots (`SalePrice` vs `Neighborhood`, `OverallQual`, etc.)

---

### 📌 Key Insights

* `OverallQual`, `GrLivArea`, `GarageArea`, and `TotalBsmtSF` are **strongly correlated** with `SalePrice`
* Several columns have significant **missing values** (e.g., `PoolQC`, `Fence`, `MiscFeature`)
* `SalePrice` is **right-skewed**, but becomes more linear and normally distributed when log-transformed
* **Outliers** exist in both `GrLivArea` and `SalePrice` — likely candidates for removal or treatment

---

### 🛠️ Tools & Libraries

* Python 3.x
* `pandas`, `numpy`
* `matplotlib`, `seaborn`

---

 

### 📘 Credits

* Dataset from [Kaggle](https://www.kaggle.com/c/house-prices-advanced-regression-techniques)
* Inspired by best practices in data science EDA and competition-winning notebooks

---
 
