# School_District_Analysis

## Overview of the school district analysis
The students data shows evidence of academic dishonesty in the math and reading scores for Thomas High School, Ninth graders and it appears to have been altered. The school wants to uphold state-testing standards. We will replace the math and reading scores for Thomas High School with NaNs while keeping the rest of the data intact. Once the math and reading scores are replaced, we can repeat the school district analysis.

## Resources
I used the following version of softwares; Anaconda(python data) 4.8.5 Python 3.7.6 Pandas and numpy for python using Jupyter notebook Finally updating the code to Github using Gitbash.

## Results
#### 1. Below data and analysis shows how the district summary is affected.

For the district summary we have used school_data_complete_df dataframe which was obtained by merginng the two dataframes; school_data_df and student_data_df. Since we have the 9th grade math and reading scores of Thomas High school replaced with Nan , this has changed the district summary analysis. The following points below explain the changes in the district.

##### a. The average reading score and average math score
The average reading score changed from 81.87 to 81.85 and the average math score changed from 78.98 to 78.93. These average scores were reduced because the 9th grade math and reading scores were replaced by NaN. The reference image link is score_comparison

##### b.The number of students that are in ninth grade at Thomas High School, the total student count and the new total student count
This data is calculated by assigning the below variables to get the output as follows ninth_grade_Thomas_High_School = 461
student_count = 39170
new_total_student_count = 38709 
New_total_count.png file for reference

##### c. Passing reading count and passing math count
The student count of Passing reading score changed from 33610 to 33158 and Passing math score changed from 29370 to28939. Since the 9th grade data with Nan is not part of the district summary now the above scores have reduced.
passing_for_module.png and passing_for_challenge

##### d. Calculate the passing reading percenatge and the passing math percentage
The passing percentages have also been changed for reading from 85.80% to 85.65% and for math from 74.98% to 74.76% .As the reading scores reduced the passsing percetages also reduced as they are directly proportional.
percentage_for_module.png and percentage_for_challenge.png

##### e. Overall passing percentage
The overall passing percentage has changed form 65.17% to 64.85% 
overall_percentage_module.png and overall_percentage_challenge.png

##### f. Final changed district summary.
Applying all the above changes in the district summary file.
District_summary_module_challenge.png-2

#### 2. Below data and analysis shows how the school summary is affected.
We have the new dataframe per_school_summary_df and this did not reflect the changes that happened in the Thomas High School, and in order to update this dataframe we have done some calculations as below.

##### a. The number of 10th-12th graders from Thomas High School.
thomas_10_12_graders = 1174

##### b. All the students passing math from Thomas High School
thomas_passing_math_df = 1094

##### c. All the students passing reading from Thomas High School
thomas_passing_reading_df = 1139

##### d. All the students passing math and reading from Thomas High School
thomas_total_passing_df = 1064

##### e. The percentage of 10th-12th grade students passing math, reading from Thomas High School and the overall passing percentage of 10th-12th grade from Thomas High School.
thomas_passing_math_percentage = 93.18 thomas_passing_reading_percentage = 97.01 thomas_overall_passing_percentage = 90.63
All the above findings can be seen in Thomas_info.png

##### f.The above data is now reflected in the per_school_summary_df by updating the dataframe.There is change in the data for Thomas High School
school_summary_thomas.png

#### 3. How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
We have calculate the top 5 schools and the bottom 5 school, Thomas High school was on the 2nd rank in the top 5 schools list in the module, however there have been changes in the school data as the math and reading scores for 9th grade have been marked as Nan but these changes did not affect the overall ranking of Thomas High school. It still holds 2nd position in the analysis. schools_top5_challenge.png

#### 4. Replacing the ninth-grade scores affect the following:
##### a. Math and reading scores by grade
Since the Thomas High school 9th grade reading and math scores have been replaced by Nan this will reflect in the data, where as the scores for other grades did not change.

##### b. Scores by school spending
We have divided the schools in groups depending on the calculated spending ranges as group_names = ["<$584", "$585-629", "$630-644", "$645-675"] and Thomas High school belongs to the group $630 - 644

The overall passing spending per student did not change as this data is not inclusive of the grades.
However there is a change in the spending range $630 - 644 because Thomas High school is part of this group
This change in range $630 - 644 is very small as the number of 9th grade students of Thomas High School make up to a very small percentange of the total students in this group and this change is not reflected when the data is rounded up.

##### c. Scores by school size
We have divided the schools in another group by the school size as group_names = ["Small (<1000)", "Medium (1000-2000)", "Large (2000-5000)"] and and Thomas High school belongs to the group "Medium (1000-2000)".

There is small change in the group "Medium (1000-2000)" because Thomas High School is part of this group.
This change is relatively small as the number of 9th grade students of Thomas High School make up to a very small percentange of the total students in this group and this change is not reflected when the data is rounded up.

##### d. Scores by school type
We already have the school type column in the data provided which divides schools as Charter and District. -Thomas High school is a Charter school.

Since Thomas High School is part of the Charter group, there is small change in this group. As the number of 9th grade students of Thomas High School make up to a very small percentange of the total students in this group, this change is not reflected when the data is rounded up.
Summary
We have done the calculations and analysis on the school district data in this module and changing the data for the 9th grade reading and math scores of Thomas high school has shown changes in the school district data. After refactoring the code and using new variables, we have come up with the following findings.

The average reading score changed from 81.87 to 81.85 and the average math score changed from 78.98 to 78.93 for the school district.
The New_total_student_count = 38709 has been used for the further analysis by removing the students of 9th grade from the total student count. This has been done because we will not be able to perform mathematical calculations with data as NaN for the 9th grade.
The student count of Passing reading score changed from 33610 to 33158 and student count of Passing math score changed from 29370 to 28939 which further changes the passing reading percentage from 85.80% to 85.65% and passing math percentage from 74.98% to 74.76%
There is a change in the overall_passing_percentage from 65.17% to 64.85% compared to the data analyzed in the module.