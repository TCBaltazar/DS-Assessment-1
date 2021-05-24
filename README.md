READme
================

# Overview/Purpose

This RMarkdown file is intended to be viewed as the solution for the
Data Science Assessment on 24/05/2021.

The following code was used, in the beginning, to create the workspace
environment:

``` r
fmxdat::make_project(FilePath="/Users/tiagob/Documents/Masters 2021/First Semester/Data Science/DS Assessment 1",ProjNam='19776209')

Texevier::create_template(directory='/Users/tiagob/Documents/Masters 2021/First Semester/Data Science/DS Assessment 1/19776209/', template_name= 'Question 1')
Texevier::create_template(directory='/Users/tiagob/Documents/Masters 2021/First Semester/Data Science/DS Assessment 1/19776209/', template_name= 'Question 2')
Texevier::create_template(directory='/Users/tiagob/Documents/Masters 2021/First Semester/Data Science/DS Assessment 1/19776209/', template_name= 'Question 3')
```

# Question 1

``` r
knitr::opts_chunk$set(echo = FALSE, message = FALSE, warning = FALSE, fig.width = 6, fig.height = 5, fig.pos="H", fig.pos = 'H')
library(pacman)
pacman::p_load(tidyverse, jtools, Hmisc)
if(!require(lubridate)) library(lubridate)

gc() # garbage collection - It can be useful to call gc after a large object has been removed, as this may prompt R to return memory to the operating system.
```

    ##           used  (Mb) gc trigger  (Mb) limit (Mb) max used  (Mb)
    ## Ncells 2178457 116.4    4040871 215.9         NA  4040871 215.9
    ## Vcells 3719228  28.4    8388608  64.0      16384  5846938  44.7

``` r
    #loading data from CSV
df_mov <- read.csv("/Users/tiagob/Documents/Masters 2021/First Semester/Data Science/DS Assessment 1/19776209/Question 1/data/Movies.csv")
```

## Introduction

This paper attempts to address three statements, posited by a friend at
a braai. The first relates to the review platform ‘Rotten Tomatoes’,
which is claimed to be a consistently good review platform. Secondly
Disney is the most profitable lead studio, and finally whether audiences
are drawn to the highest grossing films.

## Summary Statistics

The dataset used to investigate the above claims is sourced from an
associate at Mr Video, and contains info on movie critic and grossing
data; with 74 observations in 8 variables. In our sample, the two most
common genres are comedies and romances, which are 55% and 20.3%,
respectively, of the sample movies. The average audience score is 64,
the lowest score is 35, and the highest score is 89. Whereas the mean,
lowest, and highest Rotten Tomatoes scores are 47.36, 3, and 96. Summary
statistics on the variables were generated using the below code, and can
be found in the Question 1 PDF.

## Comparing Rotten Tomatoes Reviews & Audience Reviews

![Comparing Rotten Tomatoes & Audience
Scores](README_files/figure-gfm/unnamed-chunk-3-1.png)

As we can see from Figure , a Rotten Tomatoes Score &gt; 80, does not
imply that audiences will always give the movie a rating &gt; 85. In
fact, most movies with a RT score &gt; 80, have audience scores less
than 85.

## Disney Films Profitability

![Comparing the Profitability of Lead
Studios](README_files/figure-gfm/unnamed-chunk-4-1.png)

As we can see from Figure , Disney is not the most profitable of all
leading studios. In fact, independent studios appear to be the most
profitable of all lead studios. This may be because they have lower
costs of making movies, relative to bigger studios, who although make
more gross revenue from movies, also have much higher costs.

## Audiences Attraction to High Grossing Films

![Correlation Between Audience Scores and Worldwide
Gross](README_files/figure-gfm/unnamed-chunk-5-1.png)

As can be seen from Figure , there is a significant positive correlation
between a movies worldwide gross and the score an audience gives it.

# Question 2

    ##           used  (Mb) gc trigger  (Mb) limit (Mb) max used  (Mb)
    ## Ncells 2350809 125.6    4040871 215.9         NA  4040871 215.9
    ## Vcells 4028963  30.8    8388608  64.0      16384  5986662  45.7

## Introduction

The dataset used for this particular exercise merges data on
billionaires in 70 countries. It contains 2755 observations in 7
variables, including the names of billionaires, their networth, the
source of their wealth, their rank on the millionaires list, their age,
and the industry within which they made their fortune. This discussion
will present some figures in order to better understand the
characteristics of billionaires.

## Figure 1 - Distribution of Billionaires Networth by Industry

![Distribution of Billionaires Networth by
Industry](README_files/figure-gfm/unnamed-chunk-7-1.png)

As we can see from Figure (although the x-axis labels are unclear), the
industry with the highest networth individuals is Finance and
Investments, followed closely by Technology, and Manufacturing.

## Figure 2 - Billionaires Networth in BRICS Economies

![Distribution of Billionaires in BRICS
Countries](README_files/figure-gfm/unnamed-chunk-8-1.png)

Figure allows us to see that, out of the BRICS countries, Chinese
billionaires have the greatest networth.

# Question 3

    ##           used  (Mb) gc trigger  (Mb) limit (Mb) max used  (Mb)
    ## Ncells 2390927 127.7    4040871 215.9         NA  4040871 215.9
    ## Vcells 4155068  31.8    8388608  64.0      16384  6868529  52.5

## Introduction

Purpose of the study. Variable description, exploratory analysis.

## Answers

Interpretation

## More Answers

More interpretations
