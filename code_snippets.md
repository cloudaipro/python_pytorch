```python
if __name__ == '__main__': #this test defines the test block  
  <block of statements>
```

# Progress Bar
## for .ipynb
```python
from tqdm.notebook import tqdm
for i in tqdm(range(3)):
    for j in tqdm(range(50000000)):
        pass
        # print(i," : ", j)
print("Done!")
```
```python
from tqdm.notebook import tqdm
for epoch in tqdm(range(epoch_num)):
    for i, (x, y) in enumerate(tqdm(dl)):
```
## for .py
```python
from tqdm import tqdm
for i in tqdm(range(3)):
    for j in tqdm(range(50000000), leave=False):
        pass
print("Done!")
```

# jupyter filename programmatically
```python
def get_filename_of_ipynb():
    from IPython import get_ipython
    import os
    ip = get_ipython()
    path = ''
    if '__vsc_ipynb_file__' in ip.user_ns:
        path = ip.user_ns['__vsc_ipynb_file__']

    return '.'.join(os.path.basename(path).split('.')[:-1])
```
