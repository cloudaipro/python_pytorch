https://stackoverflow.com/questions/7422453/python-change-type-of-whole-list
```python
full_time_id_range11 = list(map(np.uint16, range(train_g.time_id.min(), train_g.time_id.max() + 1)))
```
