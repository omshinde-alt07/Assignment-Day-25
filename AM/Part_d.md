# 📊 Exploratory Data Analysis (EDA) using Pandas

## 🧾 Prompt
Explain EDA steps using Pandas with examples.

---

## 📌 Output

Exploratory Data Analysis (EDA) is the process of understanding and analyzing a dataset before applying any models. It helps in identifying patterns, checking missing values, and understanding the structure of the data.

### 1. Load the Dataset
```python
import pandas as pd

df = pd.read_csv("data.csv")

df.head()        # first 5 rows
df.tail()        # last 5 rows
df.shape         # (rows, columns)
df.columns       # column names

df.isnull().sum()

df.fillna(df.mean(), inplace=True)

df.info()

df.describe()

df['column_name'].unique()
df['column_name'].value_counts()

df[df['price'] > 100]

df.groupby('category')['price'].mean()

df.sort_values(by='price', ascending=False)


'''The explanation correctly covers the main steps of EDA like loading data, exploring structure, handling missing values, and summarizing data.
Code examples are simple and easy to understand.
Important Pandas functions such as head(), describe(), and groupby() are included.
One limitation is that data visualization (graphs) is not covered, which is also an important part of EDA.
Overall, the explanation is correct and useful for beginners.
'''


'''📌 Conclusion

EDA is an important step in data analysis. Using Pandas, we can easily explore, clean, and understand the dataset before moving to further analysis or modeling. '''
