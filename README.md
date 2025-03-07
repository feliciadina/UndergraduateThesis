# Prediction Dividend Payout using Multiple Linear Regression
Felicia Dina Widyasari - Undergraduate Thesis

## Company: BBCA
### 1. Import Library
```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
```

### 2. Load Dataset
```python
df = pd.read_excel('BBCA.xlsx')
print(df.head())
```

### 3. Exploratory Data Analysis (EDA)
```python
# Correlation Matrix
variables = ['Tahun', 'Total Dividen', 'EPS', 'Debt to Equity Ratio', 'ROA', 'ROE', 'Firm Size']

correlation_matrix = df[variables].corr()
plt.figure(figsize=(10, 8))
sns.heatmap(correlation_matrix, annot=True, cmap='coolwarm', fmt=".2f")
plt.title('Correlation Matrix Perusahaan BBCA')
plt.show()
```
