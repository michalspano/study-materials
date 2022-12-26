---
title: Time Scheduling Calculations
author: Michal Špano
date: 2022-11-23
papersize: a4
fontsize: 12pt
colorlinks: true
geometry: margin=1.25cm
output: pdf_document
---

## Time Scheduling Calculations

Suppose you are working in a __project__ during some set time interval. For the interval, team members decide on a __sum of predicted times__ (including all the tasks within such time interval) labeled as $S_{pt}$. Throughout the span of the time interval, team members continuously participate to keep track of time spent on each task. Then, at the end, they add all the times (they actually spent on each task) obtaining the __sum of actual times__ labeled as $S_{at}$.

We obtain a __ratio__, say $\lambda$, where $\lambda = \cfrac{S_{at}}{S_{pt}}$. If the value of $\lambda < 1$ the team has managed to completed all the tasks earlier than predicted. On the other hand, if $\lambda > 1$, then the team has not managed to complete all the tasks as late as the predicted times (resulting in a __project overdue__). We may calculate a value, say $d$, expressing the percentage by which $S_{at}$ deviates from $S_{pt}$. Hence: $d = | \lambda - 1 | \times 100$. E.g., if, in a certain project, $\lambda = 1.05$, then the additional __project overdue__ is $5\%$. 

Moreover, the individual times can be represented as __points__ in the __Cartesian coordinate system__ via a __point-to-point__ graph. Namely, we can have a two such plots: one for the __predicted time__, the latter for the __actual time__.

A __code snippet__ example taken from `R` (one point-to-point graph):

```r
x <- seq(1, 10, length.out = 10)        # x coordinates: 1 through 10
y1 <- c(1, 10, 5, 3, 4, 5, 6, 7, 8, 9)  # dummy y1 coordinates - red color (estimate)
y2 <- c(1, 3, 1, 4, 10, 9, 8, 7, 6, 4)  # dummy y2 coordinates - blue color (actual)

# estimated time + plot
plot(x, y1, col = "red", lwd = 2,
    type = "l", xlab = "week", ylab = "hour", main = "Point-to-point Graph")

lines(x, y2, col = "blue", lwd = 2) # actual time

legend("topright", legend = c("Estimate", "Actual"),
        col = c("red", "blue"), lwd = 2)
```

\pagebreak

__Out (example):__

![Point-to-point example](https://peltiertech.com/images/2016-08/MultipleXYOneDataBlock.png)

