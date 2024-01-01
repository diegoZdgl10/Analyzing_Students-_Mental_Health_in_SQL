# Project Instructions

Explore and analyze the `students` data to see how the study reached its conclusions and gain a better understanding of it. This project will take you through some exploratory analysis before investigating a specific factor for international students. The final query is the only part of your code that will be tested.

Your project will follow these exploratory steps:

- Start by counting all of the records in the data, then all records per student type to see how the records are categorized and scored.
- Filter the data to see how it differs between the student types.
- Find the summary statistics of the diagnostic tests for all students using aggregate functions, rounding the test scores to two decimal places, remembering to use aliases.
- Repeat this to summarize the data for international students only.

Your final query:
- See if length of stay impacts the average diagnostic scores rounded to two decimal places for international students, and order the results by descending order of the length of stay.
- The final output of your query with aliases will have a total nine observation rows and four columns: `stay`, `average_phq`, `average_scs`, and `average_as`, in that order.

**Note**: Creating new cells in workspace will rename the DataFrame. Make sure that your final solution uses the name `df`.
![](dfname.png)

<br>

## RESOURCES

##### Check resources that can help you solve the problem.

### S
#### [COUNT() function](https://www.datacamp.com/tutorial/count-sql-function)

### LESSONS
#### [Grouping data](https://campus.datacamp.com/courses/intermediate-sql/sorting-and-grouping-4?ex=5)
#### [Filtering grouped data](https://campus.datacamp.com/courses/intermediate-sql/sorting-and-grouping-4?ex=9)

### CHEATSHEETS
#### [SQL Basics Cheat Sheet](https://www.datacamp.com/cheat-sheet/sql-basics-cheat-sheet)

### SLIDES
#### [ROUND() function](https://campus.datacamp.com/pdf/web/viewer.html?file=https://projector-video-pdf-converter.datacamp.com/29303/chapter3.pdf#page=14)

<br>

## GUIDES

### How to approach the project
1. Explore and understand the data
2. Filter to understand the data for each student type
3. Query the summary statistics of the diagnostics scores for all students
4. Summarize the data for international students only
5. See the impact of length of stay

### 1 Explore and understand the data
Count the number of records in the dataset to confirm you have the expected number of records, then see how many records you have for each student type. Use the aliases `total_records` and `count_inter_dom`.

### 2 Filter to understand the data for each student type
Explore the data for each student type in `inter_dom` by doing three queries that filter for the two student types represented in the table, as well as the students with unknown status (`NULL`).

### 3 Query the summary statistics of the diagnostics scores for all students
Find the summary statistics for each diagnostic test using aggregate functions. Round the averages to two decimal places and use aliases `min_phq`, `max_phq`, and `avg_phq`; repeat this structure for all tests (`_scs` and `_as`).

### 4 Summarize the data for international students only
Narrow down the results down further to see the summary statistics for international students only through filtering and grouping.

### 5 See the impact of length of stay
Write a new query to see how the length of stay of an international student impacts the average diagnostic scores rounded to two decimal places, order the results by descending order of the length of stay and use the following aliases: `average_phq`, `average_scs`, and `average_as`, in that order.
