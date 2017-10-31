---
title: Draw triangles with Rmd
authors:
- :harter
tags:
- example
created_at: 2017-10-31 00:00:00
updated_at: 2017-10-31 16:16:45.051638
tldr: An example Rmd notebook for drawing a triangle
thumbnail: images/unnamed-chunk-1-1.png
---
# Triangles

Let's build a simple triangle:


```r
suppressPackageStartupMessages(library('ggplot2'))

peak <- 10
data <- data.frame(x=0:(2*peak))
data$y <- pmin(data$x, 2*peak - data$x)
ggplot(data, aes(x=x, y=y)) + geom_line()
```

![plot of chunk unnamed-chunk-1](images/unnamed-chunk-1-1.png)
