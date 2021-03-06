---
title       : Analyzing the MTCARS Data
subtitle    : Dynamic graphing using Shiny
author      : KWR
job         : PhD
framework   : io2012    # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [] # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
--- 
<style>
.title-slide {
  background-color: #FFFFFF; /* #EDE0CF; ; #CA9F9D*/
}
</style>

## Introduction to mtcars

Mtcars is a built in dataset in R. You can see the first elements below.

```r
head(mtcars)
```

```
##                    mpg cyl disp  hp drat    wt  qsec vs am gear carb
## Mazda RX4         21.0   6  160 110 3.90 2.620 16.46  0  1    4    4
## Mazda RX4 Wag     21.0   6  160 110 3.90 2.875 17.02  0  1    4    4
## Datsun 710        22.8   4  108  93 3.85 2.320 18.61  1  1    4    1
## Hornet 4 Drive    21.4   6  258 110 3.08 3.215 19.44  1  0    3    1
## Hornet Sportabout 18.7   8  360 175 3.15 3.440 17.02  0  0    3    2
## Valiant           18.1   6  225 105 2.76 3.460 20.22  1  0    3    1
```

--- .class #s1

## The issue

We would like to start plotting the various components of the dataframe and
while we can do this without any issues using ggplot there are a few annoyances:

- The graphs are not interactive. I cannot move my mouse over a data point and
see it's value.

- The process is time consuming. Every time I change something, I have to rerun
the code and look at a static plot.

- Especially cumbersome when datasets are extremely large

---.class #s2 


## The pitch

Let's utilize the power of Shiny. This will increase efficiency.


---.class #s3

## What will it do?

- Plot variables

- Color by a a variable

- Add a simple regression line

- Color the regression line

- Implements mouse interactivity (zooming, etc...)


**The shiny app can be found here:**
http://kwr-3.shinyapps.io/mtcars/

To use the app simple click on your desired preferences on the left hand side.




