---
title: "New York"
author: "Pradeep Adhokshaja"
date: "6 December 2016"
output:
  md_document:
    variant: markdown_github
---



## Introduction

The American police departments are not only responsible for catching criminals. They form an integral part of the American Community. They handle every thing from routine tasks such as directing traffic to being first responders the the country's worst disasters.

In this project , we look at the home of the largest local police department in the USA, New York. The NYPD was founded in 1845 and it is one of the most recognizable law enforcement agencies in the world. It currently consists of around 40,000 sworn officers. In this project, using the data provided by Five Thirty Eight  we try to uncover trends.


```
## 
## Attaching package: 'dplyr'
```

```
## The following objects are masked from 'package:stats':
## 
##     filter, lag
```

```
## The following objects are masked from 'package:base':
## 
##     intersect, setdiff, setequal, union
```

```
## 
## Attaching package: 'lubridate'
```

```
## The following object is masked from 'package:base':
## 
##     date
```

```
## data.table 1.9.6  For help type ?data.table or https://github.com/Rdatatable/data.table/wiki
```

```
## The fastest way to learn (by data.table authors): https://www.datacamp.com/courses/data-analysis-the-data-table-way
```

```
## -------------------------------------------------------------------------
```

```
## data.table + dplyr code now lives in dtplyr.
## Please library(dtplyr)!
```

```
## -------------------------------------------------------------------------
```

```
## 
## Attaching package: 'data.table'
```

```
## The following objects are masked from 'package:lubridate':
## 
##     hour, mday, month, quarter, wday, week, yday, year
```

```
## The following objects are masked from 'package:dplyr':
## 
##     between, last
```

```
## Warning: package 'viridisLite' was built under R version 3.3.2
```

## Number of Police Deaths in New York  State by Year

![plot of chunk unnamed-chunk-2](figure/unnamed-chunk-2-1.png)
<p> We see that the number of officers killed in New York State exceeds the nation average from the early 1900's onwards. As the population of a region increases , the crime rate is also bound to increase. The early 1900's saw a large influx of immigrants. The great depression also occurred during this time which led to people taking extreme measures to provide for their families. Unemployment benefits did not exist back then. The depression lasted for around ten years during which unemployment  hit a all time high(25%). After this period, the second World War employed a lot of labour for the manufacturing industries. The USA was supplying about 11% of the of the Allies' needs.We also see police deaths reducing during this time</p>

## Top Departments


```
## Error in loadNamespace(name): there is no package called 'webshot'
```
<p> The  department in New York State which has the highest death count is the NYPD. We will look into this further</p<

## NYPD Deaths{.tabset}

### By Year

![plot of chunk unnamed-chunk-4](figure/unnamed-chunk-4-1.png)

<p> We see that the NYPD death counts exceeds the average death counts of the state almost all the time.</p>
### Top Causes


```
## Selecting by n
```


<table class="table table-condensed">
 <thead>
  <tr>
   <th style="text-align:left;"> cause_short </th>
   <th style="text-align:left;"> n </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:left;"> Gunfire </td>
   <td style="text-align:left;"> <span style="display: inline-block; direction: rtl; border-radius: 4px; padding-right: 2px; background-color: orange; width: 100.00%">278</span> </td>
  </tr>
  <tr>
   <td style="text-align:left;"> 9/11 related illness </td>
   <td style="text-align:left;"> <span style="display: inline-block; direction: rtl; border-radius: 4px; padding-right: 2px; background-color: orange; width: 35.61%">99</span> </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Automobile accident </td>
   <td style="text-align:left;"> <span style="display: inline-block; direction: rtl; border-radius: 4px; padding-right: 2px; background-color: orange; width: 18.35%">51</span> </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Heart attack </td>
   <td style="text-align:left;"> <span style="display: inline-block; direction: rtl; border-radius: 4px; padding-right: 2px; background-color: orange; width: 14.75%">41</span> </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Struck by vehicle </td>
   <td style="text-align:left;"> <span style="display: inline-block; direction: rtl; border-radius: 4px; padding-right: 2px; background-color: orange; width: 13.31%">37</span> </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Motorcycle accident </td>
   <td style="text-align:left;"> <span style="display: inline-block; direction: rtl; border-radius: 4px; padding-right: 2px; background-color: orange; width: 12.95%">36</span> </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Gunfire (Accidental) </td>
   <td style="text-align:left;"> <span style="display: inline-block; direction: rtl; border-radius: 4px; padding-right: 2px; background-color: orange; width: 8.63%">24</span> </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Terrorist attack </td>
   <td style="text-align:left;"> <span style="display: inline-block; direction: rtl; border-radius: 4px; padding-right: 2px; background-color: orange; width: 8.63%">24</span> </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Vehicular assault </td>
   <td style="text-align:left;"> <span style="display: inline-block; direction: rtl; border-radius: 4px; padding-right: 2px; background-color: orange; width: 6.83%">19</span> </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Assault </td>
   <td style="text-align:left;"> <span style="display: inline-block; direction: rtl; border-radius: 4px; padding-right: 2px; background-color: orange; width: 5.04%">14</span> </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Fire </td>
   <td style="text-align:left;"> <span style="display: inline-block; direction: rtl; border-radius: 4px; padding-right: 2px; background-color: orange; width: 5.04%">14</span> </td>
  </tr>
</tbody>
</table>

<p> From the above table, we see that the highest number of deaths are caused by gunfire, followed by 9/11 related illness. This is then followed by automobile accidents and heart attack.</p>

### Causes of Death by Year

![plot of chunk unnamed-chunk-6](figure/unnamed-chunk-6-1.png)

<p>Upon plotting the top three causes of Death across time, we see the gunfire occurs with a larger frequency across the years.</p>

### Titles of the officers who were killed by Year

![plot of chunk unnamed-chunk-7](figure/unnamed-chunk-7-1.png)
 <p> Most of the officers who were killed in the NYPD were patrolmen, followed by police officers. We will analyse these two titles over the years.</p>
 
### Patrolman and Police

![plot of chunk unnamed-chunk-8](figure/unnamed-chunk-8-1.png)
<p> We see that police officers started getting killed from the early 1970's onwards. This is probably because of changes in the way the public started addressing patrolling officers</p>


## Sources

https://www.lycoming.edu/schemata/pdfs/Marshall_ECON236.pdf
https://en.wikipedia.org/wiki/History_of_New_York#Civil_War_to_1900
