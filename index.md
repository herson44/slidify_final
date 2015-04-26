---
title       : Slidify_Part, Standard Error Calculator 
subtitle    : Developing Data products
author      : rhen44so
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Objectives

1. Create a simple calculator of stantadard error bases just in the population and sample size

2. Explain what is standard error

3. Explain how to read and undestand standar error



--- .class #id 

## What is the Stand Error
Is the standard deviation of the Standard Distribution of a statistical (The Cambridge Dictionary of Statistics). 

In our simple shiny app project we choose the mean as our staistical. 



--- .class #id

## How to use the shiny app

You need just two samples:
1. Sample size.
2. Population Size.

Population size can be an estimation if you believe that population is big, beacuse estandard error varies just tiny amounts by vaiations in simple size if population is big. How much is big? Take for example 100,000.

There a EXAMPLE with the fomula we use


```r
s <- 100  # Sample Size
p <- 20000  # Population Size

#Standard Error is:
sqrt(((p-s)*(1.96^2)*(0.5^2))/(s*(p-s)))
```

```
## [1] 0.098
```



--- .class #id



## How to read the standard error

In simple words, you have as a result: how many points you have as error in  the median of a distribution you previously had calculated. The units of Estandard Error are the same of the mean.

For example: if as result you get 2, and your mean was 16: you have 2 points of standard deviation from your mean. in other words the mean of population probably is between 14 and 18.

--- .class #id




