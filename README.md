# School_District_Analysis

## Project overview

This project aims to analyze data on students' funding and standardized test scores 
and showcase trends in schools' performance. The analysis results will assist the school board 
in making decisions regarding the school budgets and priorities.

The list of deliverables for the project is:

- A high-level snapshot of the district's key metrics, presented in a table format.
- An overview of the key metrics for each school is presented in a table format.
- Tables presenting each of the following metrics:
- Top 5 and bottom five performing schools, based on the overall passing rate
- The average math score received by students in each grade level at each school
- The average reading score received by students in each grade level at each school
- School performance is based on the budget per student
- School performance based on the school size 
- School performance is based on the type of school

## Resources

To realize the analysis, we are given access to students' maths and reading scores from different schools 
in the district and various information about the school they attend. The data is provided in two 
CSV files:


[schools_complete.csv](https://github.com/valerielnd/School_District_Analysis/blob/main/Resources/schools_complete.csv)

[students_complete.csv](https://github.com/valerielnd/School_District_Analysis/blob/main/Resources/students_complete.csv)

We will work with Python libraries Pandas and Numpy and Anaconda's Jupyter Notebook to do the analysis.

## Analysis Results

### School district summary

The school district summary is a high-level snapshot of the following district's key metrics:

- Total number of students: 39170
- Total number of schools: 15
- Total budget of the schools in the district: is $24,649,428.00	
- Average students math score: 79.0
- Average student reading score: 81.9
- Percentage of students who passed math: 75%
- Percentage of students who passed reading: 86%
- Percentage of students who passed math and reading: %65

![original_school_summary](https://github.com/valerielnd/School_District_Analysis/blob/main/Pictures/original_school_district_summary.png)

### Per school summary

The per school summary provides the passing percentages for math and reading for each school, 
as well as the overall passing percentage for each school. It contains the following metrics:

- School name
- School type
- Total students
- Total school budget
- Per student budget
- Average math score
- Average reading score
- Percentage of students passing math
- Percentage of students passing reading
- Overall passing percentage

As mentioned earlier, there are 15 schools in the district. While the average math score at the district level
is 79, the minimum average per school is 76.6, and the maximum is 83.8. The average reading
score per school is higher than math and is between 80.7 and 84.0. As for the overall passing percentage, while
the mean for the district is 65%, this table shows the minimum average per school is 54%, and the maximum is 
91.33%, which suggests some variability across the school.

![original_per_school_summary](https://github.com/valerielnd/School_District_Analysis/blob/main/Pictures/original_per_school_summary.png)

### The highest performing school table

The highest performing school table showcases the five highest-performing schools based on the overall 
percentage of passing students.

The best performing school is Cabrera High School, with an overall passing percentage of
91.3%. Also, we can notice that all highest-performing schools are charter schools, and they all have
an overall passing score of at least 90%.


![original_best_performing_school](https://github.com/valerielnd/School_District_Analysis/blob/main/Pictures/original_highest_school.png)

### The lowest performing school table

The lowest-performing school table showcases the five lowest-performing schools based on the overall percentage 
of passing students.

We can see that the lowest-performing school is Rodriguez High School, with an overall passing percentage of
52.9%. Also, we can notice that all lowest-performing schools are district schools, and they all have
an overall passing score of at most 53%.

![orginal_lowest_performing_school](https://github.com/valerielnd/School_District_Analysis/blob/main/Pictures/original_lowest_school.png)

### Per grade and school average math and reading scores

In the first table, we display the average math score for the grades ninth, tenth, eleventh, and twelfth 
grouped by the name of the schools.

In the second table, we display the average reading score for the grades ninth, tenth, eleventh and 
twelfth grouped by the name of the schools.

We can notice that, for each school, the average math and reading score between grades is somewhat 
consistent. There is not a significant difference between their averages scores. Also, if we compare the
average per grade for math score for each school and their average for reading score, generally, 
each grade performs better in reading than math.

![original_per_grade_math](https://github.com/valerielnd/School_District_Analysis/blob/main/Pictures/original_math_grades_score.png)

![original_per_grade_reading](https://github.com/valerielnd/School_District_Analysis/blob/main/Pictures/original_reading_grades_score.png)

### School performance based on the budget per student

In this table, to show how school spending affects score averages and passing rates, we display the 
school's average scores and passing percentages by spending ranges.

There are four spending ranges from the lowest amount ($578) to the highest amount ($655):
$585, $615, $645, and $675.

Schools that have a budget of less than $585 per student have the highest average scores 
and passing percentages.


![original_performance_budget](https://github.com/valerielnd/School_District_Analysis/blob/main/Pictures/original_school_performance_based_size.png)

### School performance based on the school size 

This table displays the schools' average scores and passing percentages by school size.

There are three size ranges :
- Small: schools that have fewer than 1,000 students
- Medium : schools that have 1,000–1,999 students
- Large : schools have 2,000–5,000 students

Schools that have fewer than 1,000 students have the highest average scores 
and passing percentages.

![original_performance_size](https://github.com/valerielnd/School_District_Analysis/blob/main/Pictures/original_school_performance_based_size.png)

### School performance based on the type of school

This table displays the schools' average scores and passing percentages by school type.

There are two types of schools: Charter and district.

Charter schools have higher average scores and passing percentages than district schools.

![original_performance_type](https://github.com/valerielnd/School_District_Analysis/blob/main/Pictures/original_school_performance_based_type.png)

## Challenge overview

Since the file students_complete.csv has been altered and the reading and math grades for Thomas High 
School ninth graders are not reliable; we repeated the school district analysis after replacing math 
and reading scores for Thomas High School with NaNs while keeping the rest of the data intact.

## Analysis results

### School district summary

When we compare the results of the first School district summary and the second summary, 
the average math score, percentages of students passing reading and math, and the overall
passing percentage decreased, whereas the average reading score did not change.

![challenge_district_summary](https://github.com/valerielnd/School_District_Analysis/blob/main/Pictures/challenge_district_summary.png)

### Per school summary

The per school summary results for all the schools except for Thomas High 
The school did not change.
 
For Thomas High School, when we do not consider the 9th-grade scores, the 
average math and reading score, the percentage of passing math 
and passing reading did not change significantly. However, the overall 
passing percentage increases from 90% to 97%.

![thomas_summary](https://github.com/valerielnd/School_District_Analysis/blob/main/Pictures/thomas_school_results.png)
### The highest performing school table

The table of highest performing schools changed. Thomas High School
became the best performing High school with an overall passing percentage
of 97%.

However, the same five high schools remain at the top, and they are all charter
schools.

![challenge_top_school](https://github.com/valerielnd/School_District_Analysis/blob/main/Pictures/challenge_top_schools.png)

### The lowest performing school table

The same five high schools remain the lowest-performing schools.

### Per grade and school average math and reading scores

The Per grade and school average math and reading scores for all the school
did not change, except we are missing the results for Thomas
High School ninth graders.

![thomas_grade_math](https://github.com/valerielnd/School_District_Analysis/blob/main/Pictures/thomas_school_grade_math.png)

![thomas_grade_reading](https://github.com/valerielnd/School_District_Analysis/blob/main/Pictures/thomas_school_grade_reading.png)

### School performance based on the budget per student

The school performance based on the budget per student report was only 
affected for the range of schools that have a budget between $631-645
per student. As we can see, the overall passing percentage increased by
1%. This value was changed because Thomas High School has a 
budget of $638 per student.

![challenge_performace_budget](https://github.com/valerielnd/School_District_Analysis/blob/main/Pictures/challenge_performance_based_budget.png)

### School performance based on the school size

School performance based on the school size

The school performance based on the school size report was only affected for 
the range of medium-sized schools. As we can see, the overall passing percentage increased by 1%. 
This value was changed because Thomas High School is a medium-sized school.

![challenge_performace_size](https://github.com/valerielnd/School_District_Analysis/blob/main/Pictures/thomas_performace_based_size.png)

### School performance based on the school type

The school performance based on the school type report was only 
affected for the charter schools. As we can see, the overall 
passing percentage increased by 1%. This value was changed because
Thomas High School is a charter school.

![challenge_performace_type](https://github.com/valerielnd/School_District_Analysis/blob/main/Pictures/thomas_performace_based_type.png)

## Summary

Overall, among the analysis we repeated, the district summary, the per school summary,
the highest performing school and the schools' performance based on budget, size and 
school's type reports were modified.
