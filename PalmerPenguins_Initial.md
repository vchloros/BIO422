---
title: "Palmer Penguins Initial Analysis"
author: "Vinny Chloros"
format: html
editor: visual
execute:
  keep-md: true
theme: darkly
---



## Palmer Penguins

(*Insert informative blurb here*)


::: {.cell}

```{.r .cell-code}
library(tidyverse)

penguins <- read_csv("https://raw.githubusercontent.com/mcduryea/Intro-to-Bioinformatics/main/data/penguins_samp1.csv")

penguins |> head()
```

::: {.cell-output .cell-output-stdout}
```
# A tibble: 6 × 8
  species island bill_length_mm bill_depth_mm flipper_length_mm body_mass_g
  <chr>   <chr>           <dbl>         <dbl>             <dbl>       <dbl>
1 Gentoo  Biscoe           59.6          17                 230        6050
2 Gentoo  Biscoe           48.6          16                 230        5800
3 Gentoo  Biscoe           52.1          17                 230        5550
4 Gentoo  Biscoe           51.5          16.3               230        5500
5 Gentoo  Biscoe           55.1          16                 230        5850
6 Gentoo  Biscoe           49.8          15.9               229        5950
# ℹ 2 more variables: sex <chr>, year <dbl>
```
:::
:::


By using the `head` function, we can see the first 6 rows of our larger data set. 