# Replication Data for: The Effect of Distrust on Government Stringency During the Covid-19 Pandemic
This document outlines the structure of the replication data. To replicate the analysis open the entire repo as an R project in R studio.

The files used to create the dissertation article are in the folder Replication Scripts. This contains the rmarkdown file used to produce the paper and do the analysis (analysis_and_paper.Rmd). Title.tex contains the latex necessary to produce the title page and abstract.

The rmarkdown scripts refers to functions defined in the functions folder, which are accessed using the `box` package. functions/ts are general functions used in the paper and functions/ap are functions used to assess the statistical assumptions. Not all functions that are defined were used in the final paper. \
\
Functions imported from other packages are also imported using the `box` package. Here is complete list of packages used and required for the replication code to run: 
- `box` (for importing individual functions from packages without clustering the namespace)
- `dplyr` (for data manipulation)
- `forcats` (helps create plots with ordered labels)
- `ggplot2` (for creating plots)
- `lme4` (main pacakge used for creating random effects models)
- `texreg` (for creating regression tables)
- `sandwich` (for clustered standard errors)
- `lmtest` (same as above)
- `lubridate` (for date manipulation)
- `magrittr` (for pipe operator)
- `readr` (importing data)
- `broom` (tidying models)
- `kableExtra` (for producing tables)
- `knitr` (used for rmarkdown)
- `sf` (used in creating of map)
- `ggsci` (for graph colouring)
- `car` (for calculation of variance inflation factors)
- `HLMdiag` (for calculation of residuals)
- `influence.ME` (for calculation of DFBETAS)

The Data folder contains the replication data. panel_data.Rdata is the file containing the replication data, the function `load_project_data()` transforms some of the columns to create the dataframe used in the analysis. panel_data.csv is a file containing a csv copy of this same data (including the transformations applied by `load_project_data()`. The Map Data folder contains the data necessary for creating the map shown in the paper.
