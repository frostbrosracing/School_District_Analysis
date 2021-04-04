# A Comprehensive Analysis of a School District

## Project Overview of the District Analysis
#### This project was completed to provide insights to school district administrators about performance trends and patterns among high schools in the district.  
In order for key personnel to make strategic decisions at the school and district level, a wide range of data were collected and evaluated.  Once completed, it was discovered that there was evidence of academic dishonesty involving both the math and reading scores within a grade level at one of the high schools in the district.  Because of this, it was necessary to repeat the analysis with those suspect scores being removed from the results and the rest of the data remaining intact.  The scope of this project included the following summaries:
  1.  An overall district summary
  2.  A per school summary reflecting the highest and lowest performing schools
  3.  A summary of the math  and reading scores by grade
  4.  A summary of scores by school spending
  5.  A summary of scores by school size
  6.  A summary of scores by school type 
#### Resources
- Data Source: schools_complete.csv, students_complete.csv
- Software: Python 3.7.9, Jupyter Notebook 6.1.4, Pandas 1.1.3, Numpy 1.17.0
 
## School District Analysis Results
The results of the repeated analysis were summarized in two different ways.  
1.  The *first method* was to assign ***NaN*** for all 9th grade Thomas High reading and math scores and calculate that school's averages with only the scores from the remaining student count.  
2.  The *second method* was to assign ***NaN*** for all 9th grade Thomas High reading math scores and calculate that schools averages based on the entire student count.  

### 1. District Summary

Because this summarizes the results for over 39,000 students, the omitted grades didn't have a significant effect on the overall district analysis.  Shown below are district summaries of the original and repeated analysis.

![district_summary.png](https://github.com/frostbrosracing/School_District_Analysis/blob/main/Resources/district_summary.png)

### 2. Per School Summary by Ranking within the District
By replacing the ninth graders' math and reading scores with ***Nan***, Thomas High School's performance relative to the other schools in the district was either unaffected, or it fell significantly.  Thomas High School ranked second in the district in the original analysis and after the student count was adjusted according to the *first method*.  However, by using the *second method* of calculating the district results, Thomas High School fell to eighth place (the bottom of the list for charter schools).

As you can see from the image below, the results don't vary much when the student count is adjusted.  The overall passing percentage is within ***0.32%***.

![per_school_summary_1.png](https://github.com/frostbrosracing/School_District_Analysis/blob/main/Resources/per_school_summary_1.png)

The results differ greatly when the full student count of Thomas High is considered in the calculations as shown below.  The overall passing percentage falls by almost ***26%***.

![per_school_summary_2.png](https://github.com/frostbrosracing/School_District_Analysis/blob/main/Resources/per_school_summary_2.png)

### 3. Math and Reading Scores Summarized by Grade
The image below shows that the 9th grade Thomas High School scores for Math and Reading have been replaced by ***NaN***.

![scores_by_grade_summary.png](https://github.com/frostbrosracing/School_District_Analysis/blob/main/Resources/scores_by_grade_summary.png)

### 4. Overall Scores Summarized by School Spending
Thomas High School has a spending budget of $638 per student.  The spending brackets are binned according to the image below.  As you can see, Thomas High School falls right in the middle of the $630 - $644 per student range.  The top represents the original analysis.  The middle represents the repeated analysis according to *method 1*. The bottom represents the repeated analysis according to *method2*.

![scores_by_school_spending.png](https://github.com/frostbrosracing/School_District_Analysis/blob/main/Resources/scores_by_school_spending.png)


The 9th grade Thomas High School scores that were omitted were in-line with the scores from the rest of that school.  Because of this, when making a correction to the Thomas High School results, the  overall district analysis was left largely unaffected.  As seen in the Per School Summary original results versus adjusted results, the overall percentages were within tenths of a percent of each other.  However, if you look at the Per School Summary without the student count being corrected the numbers are quite different.  
