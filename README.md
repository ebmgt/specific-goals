# Creating specific clinical goals

This project is to create and validate a [web-based calculator](http://qitools.github.io/benchmarking/) to estimate the 50th, 75th, 80, 90th percentile performance based on published best and typical practice.

## Example
Estimating benchmarks for controlling high blood pressure using national typical and best rates of control:
* A 50th percentile of a rate of control is 64.67% (round to 65%) as provided by the federal [Quality Program Plan (QPP)](https://qpp.cms.gov/mips/explore-measures/quality-measures?search=pressure) 2019 Electronic clinical quality measures (eCQMs) data file (a copy is in the data directory above).
* A upper level for control of 90% was published by Kaiser Permanente Northern California (PMID [26939059](http://pubmed.gov/26939059)) 

Using the calculations of Hozo (Hozo, 2015; PMID [15840177](http://pubmed.gov/15840177)), the [online calculator](http://qitools.github.io/benchmarking/) estimates:
```
75th percentile (z = 0.67): 73.38
80th percentile (z = 0.84): 75.50
90th percentile (z = 1.30): 81.25
```
Thus, a clinic that wants to provide better than avareage care may decide to aim for a rate of control of 70% or 75%.

## Validation
Validation of this using [MN Community Measurement (MNCM)](https://mncm.org/reports-and-websites/reports-and-data/health-care-quality-report/)'s [Quality of Care for Chronic Conditions in Minnesota](https://mncm.org/reports-and-websites/reports-and-data/quality-of-care-for-chronic-conditions-in-minnesota/) [2018 Report](http://mncm.org/wp-content/uploads/2019/03/mncm-quality-report-2019.pdf) for Minnesota.
* Data files in Data directory above
* MCMN provides the mean, max and 90th percentile benchmarks for their measures
* In our validation, we measure the mean difference between Minnesota's reported 90th percentile and our calculated percentile using their mean and maximum rates. We used all of the Minnesota Statewide Results for Primary Care Measures.
  
rbadgett@kumc.edu

-------------------------------

[Edit this page](../../edit/master/README.md) - [History](../../commits/master/README.md)  - 
[Issues and comments](../../issues?q=is%3Aboth+is%3Aissue)
