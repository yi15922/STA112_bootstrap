HW 09 - Bootstrapping the GSS
================
Team yiit
2018-11-03

### Load packages

``` r
library(infer)
library(tidyverse)
```

### Load data

``` r
gss2016 <- read_csv("gss2016.csv")
```

### Set seed

``` r
set.seed(12354)
```

### Exercise 1

``` r
gss2016 %>%
  count(harass5)
```

    ## # A tibble: 6 x 2
    ##   harass5                                                     n
    ##   <chr>                                                   <int>
    ## 1 Does not apply (i do not have a job/superior/co-worker)    96
    ## 2 Don't know                                                  1
    ## 3 No                                                       1136
    ## 4 No answer                                                   7
    ## 5 Not applicable                                           1390
    ## 6 Yes                                                       237

The possible responses to this question is Does not apply (i do not have
a job/superior/co-worker), Don’t know, No, No answer, Not applicable,
and Yes. The number of people who said each resposne is 96, 1, 1136, 7,
1390, and 237 respectively.

### Exercise 2

``` r
harassed <- gss2016 %>%
  filter(harass5 == "Yes" | harass5 == "No")
```

### Exercise 3

### Exercise 4

### Exercise 5

### Exercise 6

### Exercise 7

### Exercise 8

### Exercise 9

``` r
gss2016 %>%
  mutate(emailmin_week = 60*as.numeric(emailhr) + as.numeric(emailmin)) %>%
  select(emailmin_week)
```

    ## Warning in evalq(60 * as.numeric(emailhr) + as.numeric(emailmin),
    ## <environment>): NAs introduced by coercion
    
    ## Warning in evalq(60 * as.numeric(emailhr) + as.numeric(emailmin),
    ## <environment>): NAs introduced by coercion

    ## # A tibble: 2,867 x 1
    ##    emailmin_week
    ##            <dbl>
    ##  1           720
    ##  2            30
    ##  3            NA
    ##  4            10
    ##  5            NA
    ##  6           120
    ##  7          2400
    ##  8            NA
    ##  9             0
    ## 10            NA
    ## # ... with 2,857 more rows

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
