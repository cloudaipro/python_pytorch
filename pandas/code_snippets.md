# How to group a Series by values in pandas?
```python
grouped = s.groupby(s)
```
Or:
```python
grouped = s.groupby(lambda x: s[x])
```
