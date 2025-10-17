Midterm Project
================

Mahitha Jangeti 10/22/25

``` r
library(tidyverse)
```

    ## ── Attaching core tidyverse packages ──────────────────────── tidyverse 2.0.0 ──
    ## ✔ dplyr     1.1.4     ✔ readr     2.1.5
    ## ✔ forcats   1.0.0     ✔ stringr   1.5.1
    ## ✔ ggplot2   3.5.2     ✔ tibble    3.3.0
    ## ✔ lubridate 1.9.4     ✔ tidyr     1.3.1
    ## ✔ purrr     1.1.0     
    ## ── Conflicts ────────────────────────────────────────── tidyverse_conflicts() ──
    ## ✖ dplyr::filter() masks stats::filter()
    ## ✖ dplyr::lag()    masks stats::lag()
    ## ℹ Use the conflicted package (<http://conflicted.r-lib.org/>) to force all conflicts to become errors

``` r
library(readxl)
library(haven)
library(dplyr)
library(ggridges)    
library(patchwork)
```

## Problem 1

``` r
mtp_df = 
  read_excel("./mtp_data/mtp_data.xlsx") %>% 
  janitor::clean_names() 
```

    ## New names:
    ## • `` -> `...2`
    ## • `` -> `...7`
    ## • `` -> `...8`
