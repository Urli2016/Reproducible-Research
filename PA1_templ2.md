# Reproducible Research - Peer Assessment 1 - 2nd Attempt
Urli2016  
January 15, 2016  

LOADING & PREPROCESSING THE DATA


```r
activity <- read.csv("activity.csv", colClasses = c("numeric", "character", 
    "numeric"))
head(activity)
```

```
##   steps      date interval
## 1    NA 10/1/2012        0
## 2    NA 10/1/2012        5
## 3    NA 10/1/2012       10
## 4    NA 10/1/2012       15
## 5    NA 10/1/2012       20
## 6    NA 10/1/2012       25
```


```r
names(activity)
```

```
## [1] "steps"    "date"     "interval"
```


```r
library(lattice)
```

```
## Warning: package 'lattice' was built under R version 3.2.2
```

```r
activity$date <- as.Date(activity$date, "%Y-%m-%d")
```
