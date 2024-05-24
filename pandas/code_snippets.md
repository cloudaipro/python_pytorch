# How to group a Series by values in pandas?
```python
grouped = s.groupby(s)
```
Or:
```python
grouped = s.groupby(lambda x: s[x])
```

# set level name of multi-index
```python
parameters_db.data.columns.set_names("signal", level=0, inplace=True)
```

#set level value of multi-index
```python
 level0 = parameters_db.data.columns.levels[0].values
level0[27] = "awesome"
level0[28] = "squeeze"
parameters_db.data.columns.set_levels(level0, level=0)
```
