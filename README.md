# City School District Standardized Test Score Analysis
## Overview
Maria is a chief data scientist for a city school district.  She has been tasked with analyzing standardized math and reading test score data to give insights on trends for schools in the district.  She will consider many factors to see if there are trends in school performance.  For example, school size, type, budget per student will be considered along with the scores.  This analysis will help the school board and superintendent on making decisions on school budgets and priorities.  She found out that her initial data set had incorrect scores for the 9th grade at Thomas High School and will be running the analysis without those students in the data set.
## Results
Removing the 461 9th grade Thomas High School student reading and math scores does not have significant changes to the results.  Below are explanations and support for this claim.  

&emsp; The 9th grade students at Thomas High School had the following results before they were removed:
      
&emsp; 9th Grade Average Math Score = 83.6

&emsp; 9th Grade Average Reading Score = 83.7

&emsp; 9th Grade % Passing Math = 90.7%

&emsp; 9th Grade % Passing Reading = 94.1%

&emsp; 9th Grade % Passing Overall = 85.2%


The score average results are in line with Thomas High School's overall averages and therefore will not shift the data by removing them.  The % passing for math, reading, and overall are slightly lower for the 9th grade so the overall school percentages will decrease slightly, but the decrease is very small and will not be significant or even noticed with rounding to the nearest whole number.    


* The district summary is not significantly impacted by removing the 9th grade Thomas High School reading and math scores.  The needle moves only 0.1% or less for passing percentages and the averages move the same.

*Distric Summary Before*
     
<p >
  <img src = https://github.com/lauras521/School_District_Analysis/blob/ad03784dd1bca7c93827cb49ca64662d28855f59/Resources/District_Summary_Before.PNG>
</p>

   *Distric Summary After*

<p >
  <img src = https://github.com/lauras521/School_District_Analysis/blob/56535541c9acb4e9795a73cca0f8a11f32cc5dd3/Resources/District_Summary_After.PNG>
</p>

* The school summary is not significantly impacted by removing the 9th grade Thomas High School reading and math scores.  As mentioned above the % passing numbers decrease slightly but the decrease is not significant.

    *School Summary Before*

<p >
  <img src = https://github.com/lauras521/School_District_Analysis/blob/a9d57d42f11bcaf1111a40f05bcf96f1fa950432/Resources/Top_5_schools_before_removal.PNG>
</p>

   *School Summary After*

<p >
  <img src = https://github.com/lauras521/School_District_Analysis/blob/a9d57d42f11bcaf1111a40f05bcf96f1fa950432/Resources/Top_5_schools_after_removal.PNG>
</p>

* How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
  * Thomas High School still ranks 2nd in Overall % Passing after removing the 9th grade math and reading scores from the analysis.  

* How does replacing the ninth-grade scores affect math and reading scores by grade?
   * See the images below that show average scores by school by grade before and after the change.  You can see Thomas's overall Average Math and Reading Scores before removal were 83.4 for math and 83.85 for reading based on the school_distric_summary_df.  Since the average of the scores that were removed are very close to averages of the school with the 10th, 11th, and 12th graders added in, the data does not change significantly.  After removal the average math score for 10th-12th graders is 83.35 for math and 83.9 for reading.

Average Math Score with 9th Grade THS Scores       |  Average Math Score without 9th Grade THS Scores
:--------------------------------------------------:|:----------------------------------------------------------:
![](https://github.com/lauras521/School_District_Analysis/blob/ad03784dd1bca7c93827cb49ca64662d28855f59/Resources/average_math_score_by_school_by_grade_before_removal.PNG)  |  ![](https://github.com/lauras521/School_District_Analysis/blob/33d993acd1455cb1c280b22d5a7733d6bcc9711a/Resources/average_math_score_by_school_by_grade_after_removal.PNG)
     
Average Reading Score with 9th Grade THS Scores       |  Average Reading Score without 9th Grade THS Scores
:--------------------------------------------------:|:----------------------------------------------------------:
![](https://github.com/lauras521/School_District_Analysis/blob/33d993acd1455cb1c280b22d5a7733d6bcc9711a/Resources/average_reading_score_by_school_by_grade_before_removal.PNG)  |  ![](https://github.com/lauras521/School_District_Analysis/blob/664a88742b574b8471ae6a4ff1ddd6c680480711/Resources/average_reading_score_by_school_by_grade_after_removal.PNG)

      
* How does replacing the ninth-grade scores affect scores by school spending?
   * See the images below that show scores by school spending are not significantly impacted by removing Thomas High School 9th grade scores for reasons mentioned above. 
      
* How does replacing the ninth-grade scores affect scores by school size?
   * See the images below that show scores by school are not significantly impacted by removing Thomas High School 9th grade score for reasons mentioned above. 
      
* How does replacing the ninth-grade scores affect scores by school type?
   * See the images below that show scores by school type are not significantly impacted by removing Thomas High School 9th grade scores for reasons mentioned above. 

<p >
  <img src = https://github.com/lauras521/School_District_Analysis/blob/7d5dbde31a0d9629c5d9938dda027770df54e1d8/Resources/spending_before_after.PNG>
</p>

<p >
  <img src = https://github.com/lauras521/School_District_Analysis/blob/7d5dbde31a0d9629c5d9938dda027770df54e1d8/Resources/size_before_after.PNG>
</p>

<p >
  <img src = https://github.com/lauras521/School_District_Analysis/blob/7d5dbde31a0d9629c5d9938dda027770df54e1d8/Resources/type_before_after.PNG>
</p>

## Summary
After Maria, cleaned the data of the incorrect 9th grade scores from Thomas High School you can see from the data above the key metrics are not significantly changed.  Minor changes include:
1. The Average Math Score for Thomas High School decreased from 83.42 to 83.35.
2. The Average Reading Score for Thomas High School increased from 83.85 to 83.90
3. 461 students were pulled out of the data set
4. % Overall Passing for Thomas High School decreased from 90.94% to 90.63%.

