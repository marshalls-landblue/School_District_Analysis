# School District Test Score Analysis

## Overview of Project

### Purpose

The purpose of this analysis was to create an accurate overview of the test scores in the school district. This involved creating cleaning up the data to make it conforming and then to remove erroneous math scores from Thomas High School. Then we are able to easily calculate new totals and averages and sort the data in an applicable manner.

## Results

Replacing the invalid scores with null values had many effects on our aggregate metrics:
* The district summary showed a slightly lower % passing compared to the original dataframe
![image](https://user-images.githubusercontent.com/17416097/151742061-367e407b-8497-4040-aa5c-f1770bcb17b3.png)
* In the school summary, you can see that Thomas High School had a reasonable average math score, but the % passing was considerably low
![image](https://user-images.githubusercontent.com/17416097/151742652-d88f584f-7c0e-4613-bf3e-a53349c9f72c.png)
* After replacing the Math and Reading Score percentages for Thomas High School by removing the 9th grade statistics, you can see that their performance is much closer aligned to the other schools.
![image](https://user-images.githubusercontent.com/17416097/151742957-252953ef-cb29-46ef-94ee-9b470a448188.png)

Other changes after replacing the values:
* Math and reading scores by grade displays 'nan' for Thomas High School 9th grade scores
* The average scores for schools with spending in the range of $630-644 are a lower
* Not a huge change in scores by school size, but you can notice a small decrease in the medium size bin.
* Slight changes to scores by school type

## Summary

Updating the 9th Grade Values to NaN changed Thomas High School's reading and math average scores, because the null values aren't included in a mean. This in turn affects the other data frames we used for this analysis. Now you can see that the percent passing on each test as well as overall in the School district are now more accurate. Having these invalid scores in was skewing our view of the different spending, size, and type bins of the schools, so it is important that we caught this and updated the data.
