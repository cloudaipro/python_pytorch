```python
test_size = int(len(dataset) * validation_size)
test_data_idx = random.sample(range(0, len(dataset)), test_size)
mask = np.full(len(dataset), False)
for i in test_data_idx: mask[i] = True 
train_data = dataset[~mask]
test_data = dataset[mask]
```

or
```python
test_size = int(len(dataset) * validation_size)
test_data_idx = random.sample(range(0, len(dataset)), test_size)
mask = np.full(len(dataset), False)
mask[test_data_idx] = True
train_data = dataset[~mask]
test_data = dataset[mask]
```
**verify**
```python
print((mask[:] == True).sum())
print((mask[:] == False).sum())
```
