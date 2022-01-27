# School_District_Analysis

## Overview of Analysis 
The school board has asked Maria for a school district analysis of all the reading and math scores of all the high schools in the district. 
We completed this analysis howevever, Maria has been told there is some academic dishonesty relating to the reading and math scores in the 
ninth grade at Thomas High School. Maria has asked us to repeat the school district analysis, while replacing the math and reading scores for 
the ninth graders at Thomas High School with NaN's in order to uphold state-testing standings. 

## Results
### District Summary 
For this analysis, the first step was to replace the ninth grade math and reading scores with NaN's.
It was important to import NumPy, to help with replacing the scores with NaN's. Once we completed this by using the loc method and the np.nan function, we were then able to complete the district summmary again.
![](resources/dataframe)
The image above shows the new district summary completed. When compared to the original summary there is not much change in the outputs. The values for average math score, average reading score, % passing math, % passing reading and % overall passing, only decrease by approximately .2 % percent at the most. When rounding to the nearest whole number, the values have stayed the same. 

### School Summary 
When we moved on to complete the school summary for the average scores and % passing for each school, there is not a difference in any of the data outside of Thomas High School, because we did not change any data involving any other school.

However, we saw a large difference in regards to Thomas High Schools data. 
We created a per school summary data frame that included all of the average reading and math scores along with the overall percentage of students passing in both math and reading. We we ran this analysis with taking out the ninth graders from Thomas High School, we saw a large increase in the percentages of students passing math, reading and overall. Below is the the data frame from our initial school summary, highlighting Thomas High School:
image of schoolsummary1
Below is an image of the data frame showing our updated school summary, taking out the ninth grade scores.
image of school summary2
We can see here that the percentage of student passing reading increases by 28%, the percentage of students passing math increases by 27% and the percentage of students passing overall increases by 25%.

### Thomas High School performance relative to other schools
In our initial analysis, Thomas High School had an overall passing percentage of 65.07%, when we ran our analysis again without the ninth graders, Thomas High School's overall passing percentage increased substantially. 
Initially, Thomas High School was ranked 8th out of the fifteen schools in regards to this statistic. Now Thomas High School ranks 2nd in % Overall Passing. This can be seen in the image below, containing the data frame showing the school summary in descending order ranked by % Overall Passing. 
image of top schools summary 

### Scores per school comparison 
#### Math and Reading scores by grade
In this analysis, there is not much change in this analysis, as the other schools scores were not changed. The only difference in our data frames is in Thomas High Schools score. Specifically, the only column that changed here was the ninth grade column, here there is NaN's replaced.

#### Scores by School Spending 
Removing the ninth grade scores from the data, influeneced the school spending data frame, by increasing the % overall passing, % passing math and % passing reading. Thomas High School is in the $630-644 spending range. Since Thomas High School's passing scores increased when the ninth grade scores were removed, the average passing percentages increased in the $630-644 spending range.

#### Scores by School Size
Thomas High School is a "medium sized" school according to the different school ranges we created. Since the passing percentages increased for Thomas High School, this increased the % passing math, % passing reading and %overall passing values for the medium sized schools. 

#### Scores by School Type 
Thomas High School is a Charter school. In this data frame we looked at passing percentages related to schools that are either Charter or District schools. Since Thomas High School is a Charter school, the passing perentages (math, reading and overall) increased after removing the ninth grade scores.

## Summary 
In summary, there were four major changes that occured when completing the school district analysis after replacing the math and reading scores from ninth graders at Thomas High School, with NaN's.
The biggest change we saw was the % Overall Passing, % Passing Math and % Passing Reading significantly increased for Thomas High School. 
This change then affected the performance of Thomas High School relative to the other schools. Thomas High School moved from 8th to 2nd in the school performance rankings. There were also changes amongst our school spending, school size and school type comparisons. These dataframes were affected since the passing averages increased in the ranges that Thomas High School was categorized in. 
