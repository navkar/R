## R Programs

## References

* [The R Project](https://www.r-project.org/)

### factors 
Factors in R are stored as a vector of integer values with a corresponding set of character values to use when the factor is displayed. The factor function is used to create a factor. The only required argument to factor is a vector of values which will be returned as a vector of factor values. 

```R
user_choices <- c("yes","no","yes","maybe")
choice_factor <- factor(user_choices)
str(choice_factor)

>> Factor w/ 3 levels "maybe","no","yes": 3 2 3 1
```

Both numeric and character variables can be made into factors, but a factor's levels will always be character values. You can see the possible levels for a factor through the levels command.

```R

choice_factor_levels <- factor(user_choices, levels = c ("yes","no","maybe"))
str(choice_factor_levels)

>> using GNU R Version 3.5.0 (2018-04-23)
 
 Factor w/ 3 levels "yes","no","maybe": 1 2 1 3
  

```

### Dates in R

* Dates are represented by the Date class
* Times are represented by the POSIXct and POSIXlt class
* Dates are stored internally as the number of days since 1970-01-01
* Times are stored internally as the number of seconds since 1970-01-01

```R
x <- as.Date("1970-01-01")
print(x)
unclass(x)

>> [1] "1970-01-01"
```

