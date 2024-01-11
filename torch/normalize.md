**transform**
```python
from sklearn_pandas import DataFrameMapper
from sklearn.preprocessing import StandardScaler

scaler = StandardScaler()
dfm = DataFrameMapper([
    ('Adj Close', None),
    (['Change Rate'], scaler)
], input_df=True, df_out=True)
Y = dfm.fit_transform(MSFT_Data)
```
**inverse_transform**
```python
inversed_Y = scaler.inverse_transform(Y[['Change Rate']])
inversed_data = scaler.inverse_transform([[-1.487230]])
```
