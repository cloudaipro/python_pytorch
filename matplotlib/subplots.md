![Screenshot 2024-02-23 at 2 45 23 PM](https://github.com/cloudaipro/AI_Notes/assets/47704397/61e74a84-9403-4e23-bbe7-6136c8e16fab)

[https://simplelearn.tw/matplotlib-intro/](https://steam.oxxostudio.tw/category/python/example/matplotlib-figure-axes.html)https://steam.oxxostudio.tw/category/python/example/matplotlib-figure-axes.html

## Remove both ticks and labels from both the axes
```python
_, axes = plt.subplots(
    3,
    10,
    figsize=(12, 4),
    # subplot_kw={"xticks": [], "yticks": []},
    # gridspec_kw={"hspace": 0.1, "wspace": 0.1},
    subplot_kw=dict(xticks=[], yticks=[]),
    gridspec_kw=dict(hspace=0.1, wspace=0.1),
)
for i, ax in enumerate(axes.flat):
    c = scaled_comps[i]
    ax.imshow(c.reshape(120, 120, 3))
```
![image](https://github.com/cloudaipro/AI_Notes/assets/47704397/8cc2eefb-d44c-4907-9be3-11c88303a62f)

```python
for i in range(images.shape[0]):
    axes = plt.subplot(10, 15, i+1)
    plt.tick_params(
        left=False,
        bottom=False,
        labelleft=False,
        labelbottom=False
    )
    plt.imshow(images[i])
```
![image](https://github.com/cloudaipro/AI_Notes/assets/47704397/dde6b8c1-4cff-42dd-8ad3-e659e1255900)


