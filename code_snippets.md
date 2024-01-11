Check the value of the built-in variable  **__name__**. This string variable is automatically created and is always defined when Python runs. (Try putting print(__name__) inside one of your  programs or type it in an interactive session.) Inside an imported module,  __name__ holds the name of the module, whereas in the main program its  value is "**__main__**".
```
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
from tqdm.notebook import tqdm
for i in tqdm(range(3)):
    for j in tqdm(range(50000000), leave=False):
        pass
        # print(i," : ", j)
print("Done!")
```
