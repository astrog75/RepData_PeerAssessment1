# Reproducible Research: Peer Assessment 1


## Loading and preprocessing the data

```r
unzip("activity.zip");
activity = read.csv("activity.csv", header = T, 
                                    comment.char = "", 
                                    na.strings = "NA",
                                    colClasses = c("integer", "factor", "integer"));
# Transform the dates into R date object
temp = as.Date(activity$date, format = "%Y-%m-%d");
activity$date = temp;
rm(temp);
```


## What is mean total number of steps taken per day?



## What is the average daily activity pattern?



## Imputing missing values



## Are there differences in activity patterns between weekdays and weekends?
