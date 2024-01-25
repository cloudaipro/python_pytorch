**display setting**
```
pd.options.display.max_columns = None
pd.options.display.expand_frame_repr = False
```

**How to Suppress Scientific Notation in Pandas**
```python
pd.options.display.float_format = '{:.0f}'.format
pd.options.display.float_format = '{:.2f}'.format
```
#### How to display all rows from dataframe using Pandas?
```python
pandas.set_option('display.max_rows', None)
```
or
```python
with pd.option_context('display.max_rows', None,):
    print(gen_analysis_data(ticks_data[0]).head(100))
```

