# 🍷 Exploratory Data Analysis (EDA) on Red Wine Quality Dataset

## 📌 Overview
This project performs **Exploratory Data Analysis (EDA)** on the Red Wine Quality dataset to understand the distribution, correlations, and key insights that impact wine quality.

## 📊 Dataset Information
The dataset contains **physicochemical properties** of Portuguese "Vinho Verde" red wines along with their **quality ratings**. The dataset is treated as both a classification and regression problem, and feature selection is explored.

### **Attributes**
#### 🔹 Input Features (Physicochemical Tests):
1. Fixed Acidity
2. Volatile Acidity
3. Citric Acid
4. Residual Sugar
5. Chlorides
6. Free Sulfur Dioxide
7. Total Sulfur Dioxide
8. Density
9. pH
10. Sulphates
11. Alcohol

#### 🎯 Target Variable:
12. **Quality** (Score between 0 and 10)

## 🛠️ Steps Performed in EDA
1. **Loading the Dataset** 📂
   ```python
   import pandas as pd
   df = pd.read_csv('winequality-red.csv')
   ```

2. **Previewing the Data** 🧐
   ```python
   df.head()
   ```

3. **Checking Data Types & Missing Values** 📋
   ```python
   df.info()
   ```

4. **Summary Statistics** 📊
   ```python
   df.describe()
   ```

5. **Data Visualization** 📈 (e.g., histograms, box plots, correlation heatmaps)
   ```python
   import seaborn as sns
   import matplotlib.pyplot as plt

   # Correlation Heatmap
   plt.figure(figsize=(10, 6))
   sns.heatmap(df.corr(), annot=True, cmap='coolwarm')
   plt.show()
   ```

## 🔍 Key Insights
- Certain factors (e.g., **alcohol, volatile acidity, sulphates**) strongly correlate with wine quality.
- Outliers and imbalances in quality ratings impact predictive modeling.
- Feature engineering and selection could improve prediction performance.

## 🚀 How to Use This Project
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/eda-red-wine.git
   ```
2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```
3. Run the Jupyter Notebook:
   ```bash
   jupyter notebook eda.ipynb
   ```

## 📌 Future Improvements
- Perform feature engineering for better predictive modeling.
- Implement classification and regression models.
- Explore outlier detection techniques.

## 🤝 Contributing
Feel free to open an issue or submit a pull request if you have suggestions for improving this analysis! 🚀



