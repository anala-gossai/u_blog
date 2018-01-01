---
title: "On my favourite R packages"
date: 2017-12-29
author: ""
draft: false
comments: false
image: ""
menu: ""
share: true
slug: "on-r-packages"
tags: ["R"]
aliases: [
    "/2017/12/29/on-r-packages/"
]
---

[R](https://www.r-project.org/) is the statistical programming language I have used for a number of years in school and work as a Quantitative Biomedical Scientist. One reason I have enjoyed using R (particularly over [SAS](https://www.sas.com/en_us/home.html?keyword=sas&matchtype=e&publisher=google&gclid=CjwKCAiA7JfSBRBrEiwA1DWSGxVjIDxgXEQ6XCT9k9cd5ijKL78eDy3UmO6hGM0gtndJoB9TNTpXJxoCZjYQAvD_BwE), but comparably to [Python](https://www.python.org/)) is the large number of [packages](https://cran.r-project.org/web/packages/available_packages_by_name.html) available for download to enhance the scope of analyses.    

There are a set of packages I always load when starting an analysis:

+ Everything in the [`tidyverse`](https://www.tidyverse.org/): the `tidyverse` includes packages that simplify data manipulation, data cleaning, data summarisation, and graphical representation of data. It is almost a different language when compared to base R, but it is __extremely__ worthwhile to learn if you are interested in joining industry, and increases the readability of your code. 
	+ Included in the core `tidyverse` are the following packages: `readr` for data acquisition; `dplyr`, `tibble`, and `tidyr` for data manipulation and cleaning; `ggplot2` for plotting; and `purrr` to extend functional programming       
	+ Favourite functions are `\%>\%` for "piping" one code statement to another, `mutate` for deriving new variables from existing variables, and `group_by` for creating new variables or getting metrics based on a certain group in the dataset 
+ [`stringr`](https://www.rdocumentation.org/packages/stringr/versions/1.1.0): helps simplify the hassle of cleaning and deriving insight from complex strings using wrapper functions as well as regular expressions. 
	+ I primarily prefer to use `stringr` over the `grep` or `gsub` functions in base R due to it's syntax.         
	+ Favourite functions are `str_extract` to find a pattern inputted as a regular expression and extracting the matching patterns, and `str_replace` to replace the characters matching a certain pattern with those specified by the user.  
+ [`zoo`](https://cran.r-project.org/web/packages/zoo/index.html): makes it easier to format and transform dates and times. 
	+ Favourite functions are `as.yearqtr` and `as.yearmon` to to format a date into just the year and quarter or year and month, respectively       
+ [`compareGroups`](https://cran.r-project.org/web/packages/compareGroups/vignettes/compareGroups_vignette.html): allows you to compare the characteristics of one group to another group with some simple univariate statistics. 
	+ I have frequently used this package in the analysis of population level data, where one group of people are compared to another group of people in the population by basic demographics, such as the proportion of males and the distribution of ages
	+ A favourite functionality of this package is its' ability to expand to output unadjusted logistic and hazards regression models       
+ [`corrplot`](https://cran.r-project.org/web/packages/corrplot/vignettes/corrplot-intro.html): graphically displays a correlation matrix as a highly customizable heatmap, with correlation coefficiants and _P_ values overlayed on the plot if desired  

I hope some of these packages also make it onto your list of favourite R packages!            
