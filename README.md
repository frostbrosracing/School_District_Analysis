# A Comprehensive Analysis of a School District

## Project Overview of the District Analysis
#### This project was completed to provide insights to school district administrators about performance trends and patterns among high schools in the district.  
In order for key personnel to make strategic decisions at the school and district level, a wide range of data were collected and evaluated.  Once completed, it was discovered that there was evidence of academic dishonesty involving both the math and reading scores within a grade level at one of the high schools in the district.  Because of this, it was necessary to repeat the analysis with those suspect scores being removed from the results and the rest of the data remaining intact.  The scope of this project included the following summaries:
  1.  An overall district summary
  2.  A per school summary
  3.  The highest and lowest performing schools
  4.  A summary of the math scores by grade
  5.  A summary of the reading scores by grade
  6.  A summary of scores by school spending
  7.  A summary of scores by school size
  8.  A summary of scores by school type 
#### Resources
- Data Source: schools_complete.csv, students_complete.csv
- Software: Python 3.7.9, Jupyter Notebook 6.1.4, Pandas 1.1.3, Numpy 1.17.0
- 
## School District Analysis Results
The results of the repeated analysis were summarized in two different ways.  The first method was to assign ***NaN*** for all 9th grade Thomas High reading and math scores and calculate that school's averages with only the scores from the remaining student count.  The second method was to assign ***NaN*** for all 9th grade Thomas High reading math scores and calculate that schools averages based on the entire student count.  

#### 1. District Summary

Because this summarizes the results for over 39,000 students, the omitted grades didn't have a significant effect on the overall district analysis.  Shown below are district summaries of the original and repeated analysis.
![district_summary.png](https://github.com/frostbrosracing/School_District_Analysis/blob/main/Resources/district_summary.png)

As you can see from the image below, the results don't vary much when the student count is adjusted.  The overall passing percentage is within ***0.32%***.
![per_school_summary_1.png](https://github.com/frostbrosracing/School_District_Analysis/blob/main/Resources/per_school_summary_1.png)
The results differ greatly when the full student count of Thomas High is considered in the calculations as shown below.  The overall passing percentage falls by almost ***26%***.
![per_school_summary_2.png](https://github.com/frostbrosracing/School_District_Analysis/blob/main/Resources/per_school_summary_2.png)



The 9th grade Thomas High School scores that were omitted were in-line with the scores from the rest of that school.  Because of this, when making a correction to the Thomas High School results, the  overall district analysis was left largely unaffected.  As seen in the Per School Summary original results versus adjusted results, the overall percentages were within tenths of a percent of each other.  However, if you look at the Per School Summary without the student count being corrected the numbers are quite different.  
