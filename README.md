# School_District_Analysis

## Purpose
A school district asked for a snapshot of several key metrics by each school campus and by the district level.  The main analysis focused on the performance of math and reading scores disaggregated several ways in preparation for a board meeting.  However, after the school board reviewed the data, it was determined that the data from Thomas High School's 9th grade class was suspect of academic dishonesty.  The school board asked for the data to be removed and analyzed again for a comparison.

### How is the district summary affected?
Original Analysis:

![](https://github.com/aem-saidur-rahman/School_District_Analysis/blob/main/Resources/original_dist_sum.png)

 461 Thomas High School 9th graders data was turned into null data, which recalculated the percentages of passing math, passing reading, and the overall passing.  The total count of students did not change as that was run on the count of the student ids, which was not turned into null data. 

Adjusted Analysis:

![](https://github.com/aem-saidur-rahman/School_District_Analysis/blob/main/Resources/adj_dist_sum.png)

When comparing the two charts, removing less than 500 test scores had a nominal impact on the almost 40,000 student data set.  The change was less than a 1% difference and the numbers would still round to the same whole number.  

### How is the school summary affected?

In the original analysis, Thomas High School started with a 91% overall passing rate, which was a concern to the school board as being too high.  After calculating the total number of 10th - 12th grade students as the new denominator, the rest of the testing data was adjusted accordingly.  

Original Analysis:

![](https://github.com/aem-saidur-rahman/School_District_Analysis/blob/main/Resources/org_sch_sum.png)

Adjusted Analysis:

![](https://github.com/aem-saidur-rahman/School_District_Analysis/blob/main/Resources/adj_sch_sum.png)

Removing the 9th grade students from the data set had a huge impact by dropping from 91% to 65% for the overall passing rate. 

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
In the original analysis, Thomas High School ranked 2nd in the district raising red flags with the school board. 

Original Analysis:

![](https://github.com/aem-saidur-rahman/School_District_Analysis/blob/main/Resources/org_ths_9.png)

After adjusting the 9th grade data, Thomas High School ranked in the exact middle of 15 campuses at 8th from the bottom. 

Adjusted Analysis:

![](https://github.com/aem-saidur-rahman/School_District_Analysis/blob/main/Resources/adj_ths_9.png)

## How does replacing the ninth-grade scores affect the following:

### Adjusted Averages using the Math and Reading Scores 

In the original analysis, Thomas High School had 83.6 math average and 83.7 reading average for the 9th grade tests. 
Now the scores have been replaced with null values and shows up in Python programming as NaN in the following charts. 

      Adjusted Average Math Scores----------------------------------------------------Adjusted Average Reading Scores

![](https://github.com/aem-saidur-rahman/School_District_Analysis/blob/main/Resources/adj_math_by_grade.png)      ![](https://github.com/aem-saidur-rahman/School_District_Analysis/blob/main/Resources/adj_read_by_grade.png)

### Scores by school spending

Thomas High School falls in the $630-$644/student spending range.  

**Original**

![](https://github.com/aem-saidur-rahman/School_District_Analysis/blob/main/Resources/org_spend.png)

There was no spending impact by changing the 9th grade scores.

**Adjusted**

![](https://github.com/aem-saidur-rahman/School_District_Analysis/blob/main/Resources/adj_spending.png)

### Scores by school size
Thomas High School is defined as a medium sized school.  The hundredths place was needed to see the nominal changes.

Original Analysis:

![](https://github.com/aem-saidur-rahman/School_District_Analysis/blob/main/Resources/org_size.png)

Adjusted Analysis:

![](https://github.com/aem-saidur-rahman/School_District_Analysis/blob/main/Resources/adj_size.png)

There was very little impact by campus size due to changing the 9th grade scores. 

### Scores by school type

Thomas High School is a charter school type. The hundredths place was needed to see the nominal changes.

Original Analysis:
![](https://github.com/aem-saidur-rahman/School_District_Analysis/blob/main/Resources/org_type.png)

Adjusted Analysis:
![](https://github.com/aem-saidur-rahman/School_District_Analysis/blob/main/Resources/adj_type.png)

There was very little impact by school type by changing the 9th grade scores. 

## Summary: Summarize four major changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.

1. The overall passing rate for Thomas High School changed drastically from 91% to 65%. 

2. Thomas High School's ranking dropped from 2nd to 8th in the district of 15 campuses. 

3. Data at the grade level will now show as "NaN" in reports for the 9th grade students at Thomas High School  

4. In addition to the overall passing rate, the campus math and reading averages and passing percentages all saw shifts.  

The major changes will be seen at the lower views of the disaggregated data with minor impact to the larger data views.
