HW 09 - Bootstrapping the GSS
================
Team Awesome
2018-10-25

### Load packages

``` r
library(infer)
library(tidyverse)
```

### Load data

``` r
<<<<<<< HEAD
gss <- read_csv("gss2016.csv", guess_max = 1000)
=======
gss2016 <- read_csv("data/gss2016.csv")
>>>>>>> 8b1f0b45858d9d2837454a8943907190a7c0392d
```

### Set seed

``` r
set.seed(12354)
```

(Add code chunks, exercise headings, and narrative as needed below.)

### Exercise 1

``` r
gss2016 %>%
  select(harass5)
```

    ## # A tibble: 2,867 x 1
    ##    harass5       
    ##    <chr>         
    ##  1 Not applicable
    ##  2 Not applicable
    ##  3 No            
    ##  4 Not applicable
    ##  5 No            
    ##  6 Not applicable
    ##  7 Not applicable
    ##  8 No            
    ##  9 Not applicable
    ## 10 No            
    ## # ... with 2,857 more rows

### Exercise 2

### Exercise 3

### Exercise 4

### Exercise 5

### Exercise 6

### Exercise 7

### Exercise 8

### Exercise 9

### Exercise 10

### Exercise 11

### Exercise 12

### Exercise 13

### Exercise 14

### Exercise 15

### Exercise 16

### Exercise 17

### Exercise 18

### Exercise 19
