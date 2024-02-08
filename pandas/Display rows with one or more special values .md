You can use DataFrame.any with parameter axis=1 for check at least one True in row by DataFrame.isna with boolean indexing:
```python
df1 = df[df.isna().any(axis=1)]
```
check at least one True in row by  == ? with boolean indexing
```python
df1 = df[(df == 0).any(axis=1)]
```
```python
def is_contained(df, special_value):
    # import pandas as pd
    if type(df).__name__ == "DataFrame":
        indices = (df == special_value).any(axis=1)
        return len(df[indices]) > 0
    else:
        return (df == special_value).any()
```

or  
Pandas Check Column Contains a Value in DataFrame  
https://sparkbyexamples.com/pandas/pandas-check-column-contains-a-value-in-dataframe/#google_vignette
