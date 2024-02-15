**How to set max output width in numpy?**
```python
np.set_printoptions( threshold=20, edgeitems=10, linewidth=140,
    formatter = dict( float = lambda x: "%.3g" % x ))  # float arrays %.3g
```
