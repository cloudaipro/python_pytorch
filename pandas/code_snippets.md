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

# xs
```python
stats = parameters_db.data.describe()
f1_stat = stats.xs(("best_f1", "f1"), level=["metrics", "results"], axis=1).T.loc[
    :, ["mean", "max"]
]
```

# drop columns
```python
parameters_db.data.drop(["c_ER_DOWNZONE_BULL", "c_ER_DOWNZONE_BEAR"], level='signal', axis=1, inplace=True)
```

# drop duplicate data
```python
index_of_unique = fbc_df.astype(str).drop_duplicates().index
purify_fbc_df = fbc_df.loc[index_of_unique].reset_index(drop=True)
```
# Get the row with the maximum value by group
```python
best_signals_parameters_df = pd.DataFrame(columns=cleaned_signals_parameters_df.columns)
for name, group in grouped_signals:
    best_signals_parameters_df = best_signals_parameters_df._append(
        group.loc[group["recall"].idxmax()]
    )
```

# check if any column is na
```python
signals_performance[signals_performance.isna().any(axis=1)]
```

# Convert index to datetime index
```python
signal_of_stks[symbol].index = pd.to_datetime(
                            signal_of_stks[symbol].index
                        )
```

# idx contain substring
```python
signal_performances_by_precision[(signal_performances_by_precision.index.str.contains("c_RSX")) | (signal_performances_by_precision.index.str.contains("c_CMO"))]
```

# concat list fields
```python
all_signals = list(itertools.chain(*signals_performance.signals.values))
```
# Comparison between datetime and datetime64[ns] in pandas
```python
    short_csm_ta_data = {k: v[v.index > pd.Timestamp(six_months_ago)] for k, v in csm_ta_data.items()}
```
