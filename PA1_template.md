
 ## Are there differences in activity patterns between weekdays and weekends?
-##### 1.Create a new factor variable in the dataset with two levels – “weekday” and “weekend” indicating whether a given date is a weekday or weekend day.
+##### 1. Create a new factor variable in the dataset with two levels – “weekday” and “weekend” indicating whether a given date is a weekday or weekend day.
 
 
 ```r
 activityDataImputed$dateType <-  ifelse(as.POSIXlt(activityDataImputed$date)$wday %in% c(0,6), 'weekend', 'weekday')
 ```
 
-##### 2.Make a panel plot containing a time series plot
+##### 2. Make a panel plot containing a time series plot
 
 
 ```r
