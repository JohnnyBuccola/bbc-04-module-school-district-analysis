# Module 4 Challenge - School District Analysis
## Overview
After assembling the academic results for the school district, it was found that the reading and math grades for ninth graders at Thomas High School appear to have been altered.  The purpose of this task was to remove all potentially affected scores from the analysis and create a new report with the cleaned results. 
## Results
All scores from ninth graders at THS (Thomas High School) were removed from the data set and replaced with `NaN` so that they would not be included in any averages or calculations.  Here is a sample of the cleaned data, with the augmented scores highlighted:

![Image showing scores that were removed](/Images/Removed_Scores.png)

All of the district and school-focused summaries were then updated, removing the affected 461 students from the percentage and average calculations.  The following changes were identified:

* __District Summary__ - The removed scores led to minor changes on the overall district summary. The average math score was reduced by 0.1, and the average reading score was unchanged.  The % passing math, % passing reading, and % passing overall were reduced by .2%, .1%, and .3% respectively.  

* __School Summary__ - The removed scores led to minor reductions in passing rates for math, reading, and overall.  The differences can be seen in the tables below.

    Before 9th Grader Adjustment:
    ![Summary of THS before removing 9th grade scores](/Images/THS_summary_old.png)
    After 9th Grader Adjustment:
    ![Summary of THS after removing 9th grade scores](/Images/THS_summary_adjusted.png)
 
* __Relative Performance__ - THS's position as the #2 school overall by % overall passing rate was unchanged.  However, it drops into a near tie with the #3 overall school, Griffin High School.

* __Score Breakdowns__ - 
    * _Scores by Grade_ - The only change is that THS no longer has any scores for the 9th grade, as they were replaced by `NaN`
    * _Scores by School Spending_ - Removing THS 9th graders had a negligible affect on the scores in the "$630-644" spending category.
    * _Scores by School Size_ - Removing THS 9th graders had a negligible affect on the scores in the "Medium (1000-2000)" school size category.
    * _Scores by School Type - Removing THS 9th graders had a negligible affect on the scores in the "Charter" school type category.

## Summary
Removing the 9th graders' scores from the THS data set had little impact on the overall analysis of the results. This is because this group of students performed, on average, roughly the same as the students in 10th-12th grades at THS.  The only significant impact is that the _Scores by Grade_ breakdown no longer contains data for this segment.
