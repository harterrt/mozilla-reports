---
title: Draw a triangle with Python
authors:
- :harter
tags:
- example
created_at: 2017-10-31 00:00:00
updated_at: 2017-10-31 10:00:26.931112
tldr: An example notebook/function for drawing a triangle in python
thumbnail: images/output_2_0.png
---
```python
def draw_a_triangle(peak):
    for i in range(1, peak * 2):
        print '*' * (i - 2 * max(0, i-peak))

draw_a_triangle(10)
```
    *
    **
    ***
    ****
    *****
    ******
    *******
    ********
    *********
    **********
    *********
    ********
    *******
    ******
    *****
    ****
    ***
    **
    *



```python
import matplotlib.pyplot as plt

def plot_a_triangle(peak):
    X = range(1, peak * 2)
    plt.plot(X, [x - 2 * max(0, x-peak) for x in X])
    plt.show()

plot_a_triangle(10)
```


![png](images/output_2_0.png)
