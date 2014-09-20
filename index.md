---
title       : BMI Calculator
subtitle    : An easy to use calculator for BMI
author      : Christoph Schwerdtfeger
job         : Student
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : self-contained # {standalone, draft}
knit        : slidify::knit2slides
---

## Motivation

* Disclaimer: This has been prepared for educational purposes and is not meant to be used when examining health problems.

* Obesity and overweight are a growing health problem, especially in the developed world.
* BMI is an easy to use indicator to assess an adults' weight relative to their size.
* However, the math is not easy enough to be done in your head, especially if you are not used to the metric system or forgot the binomic formulas...


---

## What is BMI?

* BMI is the abbreviation for Body Mass Index
* It is calculated by dividing a person's weight by their squared height
* Example: A person weighs 78 kgs and is 1.78 meters tall:


```r
BMI <- 78 / (1.78*1.78)
BMI
```

```
## [1] 24.62
```


---

## Why do I need an online calculator?

* I forgot to mention: the weight and height have to be reported in the metric system, using meters and kilograms.
* Most people would not even know how to convert feet and inches to meters.
* Or pounds to kilograms.
* The BMI Calculator lets you chose between the metric system and the traditional U.S. measures.
* To my knowledge, all other major non-metric systems (notably the Russian and the Chinese system) have been abandoned in favor of the metric system.
* So the BMI Calculator should be able to serve most of the world.

---

## How do I interpret results?

* The World Health Organization considers a person overweight, if their BMI is 25 or above, and obese if it is 30 or above.


```r
if (BMI>=30) {
        WHO <- "The person is considered obese"
} else if (BMI>=25) {
        WHO <- "The person is considered overweight"
} else {
        WHO <- "The person is considered of normal weight"
}

WHO
```

```
## [1] "The person is considered of normal weight"
```


* For further information please refer to http://www.cdc.gov/obesity/adult/defining.html



