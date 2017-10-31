---
title: Draw a triangle with Python
authors:
- :harter
tags:
- example
created_at: 2017-10-31 00:00:00
updated_at: 2017-10-31 10:04:56.413771
tldr: An example notebook/function for drawing a triangle in python
thumbnail: images/output_2_0.png
---
```python
def draw_a_triangle(peak):
    for i in range(1, peak * 2):
        print '*' * min(i, 2 * peak - i)

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
    x = range(1, peak * 2)
    y = [min(xi, 2 * peak - xi) for xi in x]
    plt.plot(x, y)
    plt.show()

plot_a_triangle(10)
```


![png](images/output_2_0.png)
