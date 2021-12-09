Untitled
================

## GitHub Documents

This is an R Markdown format used for publishing markdown documents to
GitHub. When you click the **Knit** button all R code chunks are run and
a markdown file (.md) suitable for publishing to GitHub is generated.

## Including Code

You can include R code in the document as follows:

``` r
library(tidyr)
library(tidyverse)
```

    ## ── Attaching packages ─────────────────────────────────────── tidyverse 1.3.1 ──

    ## ✓ ggplot2 3.3.5     ✓ dplyr   1.0.7
    ## ✓ tibble  3.1.4     ✓ stringr 1.4.0
    ## ✓ readr   2.0.2     ✓ forcats 0.5.1
    ## ✓ purrr   0.3.4

    ## ── Conflicts ────────────────────────────────────────── tidyverse_conflicts() ──
    ## x dplyr::filter() masks stats::filter()
    ## x dplyr::lag()    masks stats::lag()

``` r
library(ggplot2)
```

``` r
Ma_percapita<-read.csv("Per_capita_personal_income.csv")
```

## Including Plots

You can also embed plots, for example:

`{ r percapita echo=FALSE} ggplot(data = Ma_percapita, mapping = aes(x =
name, y=per_capita_2020,fill=name)) + geom_col()+ theme(axis.text.x =
element_text(angle = 90))+ labs(title= "Percapita of MA cities in the
year 2020",x="county",y="percapita",fill="County names")`

Note that the `echo = FALSE` parameter was added to the code chunk to
prevent printing of the R code that generated the plot.
