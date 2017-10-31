---
title: Draw a triangle with Python
authors:
- :harter
tags:
- example
created_at: 2017-10-31 00:00:00
updated_at: 2017-10-31 09:46:02.396382
tldr: An example notebook/function for drawing a triangle in python
---
```python
def draw_a_triangle(peak):
    for i in range(peak * 2):
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
