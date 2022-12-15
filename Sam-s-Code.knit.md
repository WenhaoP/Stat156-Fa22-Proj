---
title: "Replication of Miguel 2004 Civil Conflict and Economic Shock"
author: "Sam Tan"
date: "2022-12-11"
output:
  pdf_document: 
    latex_engine: xelatex
    

---



## Civil Conflict



```
## New names:
## Rows: 41 Columns: 4
## -- Column specification
## -------------------------------------------------------- Delimiter: "," chr
## (2): StateAbb, StateNme dbl (2): ...1, CCode
## i Use `spec()` to retrieve the full column specification for this data. i
## Specify the column types or set `show_col_types = FALSE` to quiet this message.
## * `` -> `...1`
```



```
## # A tibble: 5 x 23
##     Primkey    ID SubID Location Side_A Side_B Incompatibility Territory    YEAR
##       <dbl> <dbl> <dbl> <chr>    <chr>  <chr>            <dbl> <chr>       <dbl>
## 1 280001992  2800     0 Niger    Niger  FLAA                 1 Air and Az~  1992
## 2 280001994  2800     0 Niger    Niger  CRA                  1 Air and Az~  1994
## 3 280001997  2800     0 Niger    Niger  UFRA                 1 Air and Az~  1997
## 4 315001996  3150     0 Niger    Niger  FDR                  1 Eastern Ni~  1996
## 5 315001997  3150     0 Niger    Niger  FARS                 1 Eastern Ni~  1997
## # ... with 14 more variables: Intensity <dbl>, Type <dbl>, Startdate <dttm>,
## #   Startprecision <dbl>, Startdate2 <dttm>, Startprecision2 <dbl>,
## #   COW_A <chr>, COW_B <chr>, COW_location <chr>, Region <dbl>, Lat <dbl>,
## #   Lon <dbl>, Radius <dbl>, Version <dbl>
```



|Country                  | Total
Years| Years of Civil Conﬂict ≥25 Deaths (PRIO/Uppsala)| Years of Civil Conﬂict ≥1,000 Deaths (PRIO/Uppsala)|
|:------------------------|----------:|------------------------------------------------:|---------------------------------------------------:|
|Angola                   |         19|                                               19|                                                  16|
|Benin                    |         19|                                                0|                                                   0|
|Botswana                 |         19|                                                0|                                                   0|
|Burkina Faso             |         19|                                                1|                                                   0|
|Burundi                  |         19|                                                8|                                                   1|
|Cameroon                 |         19|                                                1|                                                   0|
|Central African Republic |         19|                                                0|                                                   0|
|Chad                     |         19|                                               17|                                                   9|
|Congo, Brazzaville       |         19|                                                5|                                                   2|
|Congo, Kinshasa          |         19|                                                4|                                                   3|
|Cote d'Ivoire            |         19|                                                0|                                                   0|
|Djibouti                 |         19|                                                5|                                                   0|
|Ethiopia                 |         19|                                               15|                                                  11|
|Gabon                    |         19|                                                0|                                                   0|
|Gambia                   |         19|                                                1|                                                   0|
|Ghana                    |         19|                                                2|                                                   0|
|Guinea                   |         19|                                                0|                                                   0|
|Guinea-Bissau            |         19|                                                2|                                                   1|
|Kenya                    |         19|                                                1|                                                   0|
|Lesotho                  |         19|                                                1|                                                   0|
|Liberia                  |         19|                                                7|                                                   2|
|Madagascar               |         19|                                                0|                                                   0|
|Malawi                   |         19|                                                0|                                                   0|
|Mali                     |         19|                                                2|                                                   0|
|Mauritania               |         19|                                                0|                                                   0|
|Mozambique               |         19|                                               12|                                                  12|
|Namibia                  |         10|                                                0|                                                   0|
|Niger                    |         19|                                                4|                                                   0|
|Nigeria                  |         19|                                                0|                                                   0|
|Rwanda                   |         19|                                                8|                                                   3|
|Senegal                  |         19|                                                7|                                                   0|
|Sierra Leone             |         19|                                                9|                                                   2|
|Somalia                  |         19|                                               16|                                                   4|
|South Africa             |         19|                                                8|                                                   6|
|Sudan                    |         19|                                               17|                                                  15|
|Swaziland                |         19|                                                0|                                                   0|
|Tanzania                 |         19|                                                0|                                                   0|
|Togo                     |         19|                                                2|                                                   0|
|Uganda                   |         19|                                               17|                                                  10|
|Zambia                   |         19|                                                0|                                                   0|
|Zimbabwe                 |         19|                                                0|                                                   0|
|Total                    |        770|                                              191|                                                  97|

```
## # A tibble: 6 x 3
##     mean    sd   obs
##    <dbl> <dbl> <int>
## 1 0.248  0.432   770
## 2 0.0614 0.240   586
## 3 0.158  0.365   184
## 4 0.126  0.332   770
## 5 0.0267 0.161   673
## 6 0.186  0.391    97
```

# Merge data


```
## New names:
## Rows: 850 Columns: 84
## -- Column specification
## -------------------------------------------------------- Delimiter: "," chr
## (5): country.x, country.y, cname, casename, waryrs dbl (79): ...1, ccode, year,
## GPCP, GPCP_L, GPCP_L2, GPCP_G, GPCP_G_L, GPCP_G...
## i Use `spec()` to retrieve the full column specification for this data. i
## Specify the column types or set `show_col_types = FALSE` to quiet this message.
## * `` -> `...1`
```

```
## # A tibble: 10 x 3
##     year country.x ccode
##    <dbl> <chr>     <dbl>
##  1  1990 Namibia     565
##  2  1991 Namibia     565
##  3  1992 Namibia     565
##  4  1993 Namibia     565
##  5  1994 Namibia     565
##  6  1995 Namibia     565
##  7  1996 Namibia     565
##  8  1997 Namibia     565
##  9  1998 Namibia     565
## 10  1999 Namibia     565
```


```
## 
## Please cite as:
```

```
##  Hlavac, Marek (2022). stargazer: Well-Formatted Regression and Summary Statistics Tables.
```

```
##  R package version 5.2.3. https://CRAN.R-project.org/package=stargazer
```

```
## 
## % Table created by stargazer v.5.2.3 by Marek Hlavac, Social Policy Institute. E-mail: marek.hlavac at gmail.com
## % Date and time: Sun, Dec 11, 2022 - 18:00:55
## \begin{table}[!htbp] \centering 
##   \caption{} 
##   \label{} 
## \begin{tabular}{@{\extracolsep{5pt}}lccccc} 
## \\[-1.8ex]\hline 
## \hline \\[-1.8ex] 
##  & \multicolumn{5}{c}{\textit{Dependent variable:}} \\ 
## \cline{2-6} 
## \\[-1.8ex] & \multicolumn{5}{c}{GDP\_G} \\ 
## \\[-1.8ex] & (1) & (2) & (3) & (4) & (5)\\ 
## \hline \\[-1.8ex] 
##  Growth in rainfall, t & 0.055$^{***}$ & 0.055$^{***}$ & 0.054$^{***}$ & 0.058$^{***}$ & 0.053$^{***}$ \\ 
##   & (0.014) & (0.016) & (0.016) & (0.019) & (0.016) \\ 
##   & & & & & \\ 
##  Growth in rainfall, t-1 & 0.041$^{***}$ & 0.041$^{**}$ & 0.039$^{**}$ & 0.042$^{**}$ & 0.044$^{***}$ \\ 
##   & (0.015) & (0.016) & (0.016) & (0.017) & (0.016) \\ 
##   & & & & & \\ 
##  Growth in rainfall, t+1 &  & 0.008 &  &  &  \\ 
##   &  & (0.009) &  &  &  \\ 
##   & & & & & \\ 
##  Growth in terms of trade t &  & 0.0003 &  &  &  \\ 
##   &  & (0.001) &  &  &  \\ 
##   & & & & & \\ 
##  Log(GDP per capita), 1979 &  & $-$0.051 &  &  &  \\ 
##   &  & (0.034) &  &  &  \\ 
##   & & & & & \\ 
##  Democracy (Polity
##  IV), t-1 &  & 0.007 &  &  &  \\ 
##   &  & (0.041) &  &  &  \\ 
##   & & & & & \\ 
##  Ethnolinguistic fractionalization &  & $-$0.010 &  &  &  \\ 
##   &  & (0.019) &  &  &  \\ 
##   & & & & & \\ 
##  Religious fractionalization &  & 0.004 &  &  &  \\ 
##   &  & (0.007) &  &  &  \\ 
##   & & & & & \\ 
##  Oil-exporting Country &  & 0.008 &  &  &  \\ 
##   &  & (0.006) &  &  &  \\ 
##   & & & & & \\ 
##  Log(mountainous) &  &  &  & 0.008 &  \\ 
##   &  &  &  & (0.017) &  \\ 
##   & & & & & \\ 
##  Log(national popu-
##  lation), t _ 1 &  &  &  &  & $-$0.004 \\ 
##   &  &  &  &  & (0.017) \\ 
##   & & & & & \\ 
##  Constant & $-$0.007$^{**}$ & 0.005 & 0.024 & 0.024 & 0.024 \\ 
##   & (0.003) & (0.045) & (0.017) & (0.017) & (0.015) \\ 
##   & & & & & \\ 
## \hline \\[-1.8ex] 
## Country fixed effect & No & No & Yes & Yes & Yes \\ 
## Country-speciﬁc time trend & No & Yes & No & No & No \\ 
## \hline \\[-1.8ex] 
## Observations & 744 & 671 & 671 & 671 & 607 \\ 
## R$^{2}$ & 0.022 & 0.070 & 0.127 & 0.127 & 0.159 \\ 
## Adjusted R$^{2}$ & 0.019 & $-$0.004 & 0.005 & 0.004 & 0.035 \\ 
## Residual Std. Error & 0.070 (df = 741) & 0.071 (df = 621) & 0.071 (df = 588) & 0.071 (df = 587) & 0.064 (df = 528) \\ 
## F Statistic & 8.224$^{***}$ (df = 2; 741) & 0.950 (df = 49; 621) & 1.043 (df = 82; 588) & 1.031 (df = 83; 587) & 1.284$^{*}$ (df = 78; 528) \\ 
## \hline 
## \hline \\[-1.8ex] 
## \textit{Note:}  & \multicolumn{5}{r}{$^{*}$p$<$0.1; $^{**}$p$<$0.05; $^{***}$p$<$0.01} \\ 
## \end{tabular} 
## \end{table} 
## 
## % Table created by stargazer v.5.2.3 by Marek Hlavac, Social Policy Institute. E-mail: marek.hlavac at gmail.com
## % Date and time: Sun, Dec 11, 2022 - 18:00:56
## \begin{table}[!htbp] \centering 
##   \caption{} 
##   \label{} 
## \begin{tabular}{@{\extracolsep{5pt}} c} 
## \\[-1.8ex]\hline 
## \hline \\[-1.8ex] 
## Economic Growth Rate, t \\ 
## \hline \\[-1.8ex] 
## \end{tabular} 
## \end{table}
```



