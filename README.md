# School_District_Analysis

## Project overview

The purpose of this project is to analyze data on students fundings and standardized test scores 
and showcase trends in school performance. The results of the analysis will asssit the school board 
in making decisions regarding the school budgests and priorities.

The list of deliverables for the project is:

- A high-level snapshot of the district's key metrics, presented in a table format.
- An overview of the key metrics for each school, presented in a table format.
- Tables presenting each of the following metrics:
- Top 5 and bottom 5 performing schools, based on the overall passing rate
- The average math score received by students in each grade level at each school
- The average reading score received by students in each grade level at each school
- School performance based on the budget per student
- School performance based on the school size 
- School performance based on the type of school

## Resources

To realize the analysis, we are given access to students maths a reading scores from different schools 
in the district as well as various information about the school they attend. The data is given in two 
csv files:

[schools_complete.csv]()

[students_complete.csv]()

To do the analysis, we will work the Python's libraries Pandas and Numpy and Anaconda's Jupyter Notebook.

## Analysis Results

### School district summary

The school district summary is a high-level snapshot of the following district's key metrics:

- Total number of students : 39170
- Total number of schools: 15
- Total bugdet of the schools in the disctrict: $24,649,428.00	
- Average students math score : 79.0
- Average students reading score : 81.9
- Percentage of students who passed math: 75%
- Percentage of students who passed reading : 86%
- Percentahe of who students who passed math and readings : %65

![original_school_summary]()

### Per school summary

The per school summary provides the passing percentages for math and reading for each school, 
as well as get the overall passing percentage for each school. It contains the following metrics:

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

As mentioned earlier, there are 15 schools in the district. While the average math score for the district
is 79, we can see that the minumum average per school is 76.6 and the maximum is 83.8. The average reading
score per school reaches a higher range between 80.7 and 84.0. As for the overall passing percentage, while
the mean for the district is 65%, this table shows the minimum average per school is 54% and the maximum is 
91.33% which suggests some variability across school.

![original_per_school_summary]()

### The highest performing school table

The highest performing school table showcases the 5 highest-performing schools based on the overall 
percentage of passing students.

We can see that the best performing school is Cabrera High School with an overall passing percentage of
91.3. Also, we can notice that all highest-performing school are charter schools and they all have
an overall passing score of at least 90%.


![original_best_performing_school]()

### The lowest performing school table
The lowest performing school table showcase the lowest-performing schools based on the overall percentage 
of passing students.

We can see that the lowest performing school is Rodriguez High School with an overall passing percentage of
52.9%. Aslo, we can notice that all lowest-performing schools are district schools and they all have
an overall passing score of at most 53%.

![orginal_lowest_performing_school]()

### Per grade and shool average math and reading scores

In the first table, we display the average math scores for the grades ninth, tenth, eleventh and twelth 
grouped by the name of the schools.

In the second table, we display the average reading scores for the grades ninth, tenth, eleventh and 
twelth grouped by the name of the schools.

We can notice that, for each school, the average math and reading score between grades is somewhat 
consistent. There is not a large difference between their averages scores. Also, if we compare the
average per grades for math score for each scool and their average for reading score, generally 
each grade perform better in reading than math.

![original_per_grade_math]()

![original_per_grade_reading]()

### School performance based on the budget per student

In this table, to show how school spending affects score averages and passing rates, we display the 
school's average scores and passing percentages by spending ranges.

There are four spending ranges from the lowest amount ($578) to the highest amount ($655):
$585, $615, $645, and $675.

The results show schools that have a bugdet less than $585 per student have the highest average scores 
and passing percentages.

![original_performance_budget]()

### School performance based on the school size 

In this table, we display the schools average scores and passing percentages by school size.

There are three size ranges :
- Smalll : schools that have fewer than 1,000 students
- Medium : schools that have 1,000–1,999 students
- Large : schools have 2,000–5,000 students

The results show schools that have fewer than 1,000 students have the highest average scores 
and passing percentages.

![original_performance_size]()

### School performance based on the type of school

In this table, we display the schools average scores and passing percentages by school type.

There are two types of schools : Charter and district

The results show charter have higher average scores and passing percentages than district schools.

![original_performance_type]()

## Challenge overview

Since the file students_complete.csv has been altered and the reading and math grades for Thomas High 
School ninth graders are not reliable, we repeated the school district analysis after replacing math 
and reading scores for Thomas High School with NaNs while keeping the rest of the data intact.

## Analysis results

### School district summary

when we compare the results of the first summary and the second summary, 
the disctrict average math score, percentage of passing reading, the overall
passing and the percentage of passing math decreased whereas the average
reading score did not change.

![challenge_district_summary]()

### Per school summary

The per school summary results for all the schools execpt for Thomas High 
School did not change.
 
When we do not consider the 9th scores, the average math and reading score 
for Thomas High School as well as the percentage of passing math, 
and passing reading did not change significantly. However, the overall 
passing percentage increases from 90% to 97%.

### The highest performing school table

The new table of highest performing school changed. Thomas High School
became the best perfoming High school with an overall passing percentage
of 97%.

However, the same five high school remain at the top and they are all charter
schools.

![challenge_top_school]()

### The lowest performing school table

The table of lowest performing school did not chage.

### Per grade and shool average math and reading scores

The Per grade and shool average math and reading scores for all the school
did not change expect we are missing the results for ninth grade for Thomas
High School.

![thomas_grade_math]()

![thomas_grade_reading]()

### School performance based on the budget per student

The school performance based on the budget per student report was only 
affected for the range of school that have a bugdet between $631-645
per student. As we can see the overall passing percentage increased by
1%. This modification is due to the fact that Thomas High School is
one of those schools.

![challenge_performace_budget]()

### School performance based on the school size

The school performance based on the school size report was only 
affected for the range of medium size schools. As we can see the overall 
passing percentage increased by 1%. This modification is due to the fact 
that Thomas High School is one of those schools.

![challenge_performace_size]()

### School performance based on the school type

The school performance based on the school type report was only 
affected for the charter schools. As we can see the overall 
passing percentage increased by 1%. This modification is due to the fact 
that Thomas High School is one of those schools.

![challenge_performace_type]()