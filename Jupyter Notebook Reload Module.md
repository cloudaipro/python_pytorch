1. Using the reload() Function from the importlib Module
```python
import example
import importlib
# make changes to example.py file
importlib.reload(example)
```

2. Using the %load_ext and %autoreload Magic Commands
```python
%load_ext autoreload
%autoreload 2

import example
# make changes to example.py file
```
