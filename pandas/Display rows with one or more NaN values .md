You can use DataFrame.any with parameter axis=1 for check at least one True in row by DataFrame.isna with boolean indexing:
```python
df1 = df[df.isna().any(axis=1)]
```
