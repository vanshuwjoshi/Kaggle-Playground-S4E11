# Exploratory Data Analysis

Steps:

1. Exploratory Data Analysis
2. Data cleaning
3. Explanatory Analysis - Clean graphs and maybe dashboard
4. Data transformation - scaling and all
5. Model

## Columns

### 1. Gender

### 2. Age

### 3. City

### 4. Working Professional or Student

- High percentage of students feel depressed
- Count of students is small however the percentage of depressed student is near 60%.
- Number of working professionals is high but the percentage of depressed professionals is around 8%.
- Therefore, must keep this for the model - student has a high likelihood of being depressed.

### 5. Profession

- High null values
- High incorrect values
- Need to replace alot of values or remove some of them.
- Graphic designer is most likely to be depressed (around 30% of GDs feel depressed)
- While less than 2% of Entreprenuers and Content Writers feel depressed
- High number of unemployed people are depressed as well

### 6. Academic Pressure

- High null values because of people not a student anymore (need to think of this, can give 0 (but the category is ordinal))
- Academic pressure will have high correlation with Depression
- However, when doing train test split majority of the Academic pressure rows went to test data.
- So, when doing the train test split for modelling we neeed to make sure this does not happen.
- As the academic pressure goes beyond 2, more students are depressed than non-depressed.
- Therefore, we can say that academic pressure is a big factor in being depressed.

### 7. Work Pressure

- 27000 missing values, must be a lot of students and people who are not working.
- High work pressure, means high chance of being depressed

### 8. CGPA

- Can round off the values here to get integer values.
- More than 100,000 missing values.
- Near perfect CGPA (10) students have high percentage of depressed students.
- Can say that students with low CGPA and high CGPA are both at the chance of depression
- Can divide this in categories (low, medium, or high)
- No clear pattern, however.

### 9. Study Satisfaction

- High number of null values
- Lesser the study satisfaction, higher the percentage of being depressed.
- Majority of the students who have given 4 or less on study satisfaction are depressed.

### 10. Job Satisfaction

- 27000 missing values.
- Same trend as study satisfaction, lesser the job satisfaction, higher the percentage of being depressed.

### 11. Sleep Duration

- No null values.
- Need to clean this column, then visualize
- Highest number of depressed people have less than 5 hours of sleep.

### 12. Dietary Habits

- 4 null values (can remove them if they are not "depressed").
- Clean the column as well to visualize better.
- "More Healthy" -> "Healthy" and so on
- Unhealthy habits in diet may lead to high chance of depression.

### 13. Degree

- 2 null values
- Maybe can combine all 12th, bachelors, masters, phd.
- Can make them ordinal as well.
- Bad visualization. Need cleaning
- Majority of Class 12 students feel depressed.

### 14. Have you ever had suicidal thoughts ?

- No null values
- There is a high chance that people who have suicidal thought are depressed compared to people who do not have suicidal thoughts.

### 15. Work/Study Hours

- No null values
- Higher the number of hours is may lead to people being depressed.

### 16. Financial Stress

- 4 null values
- High financial stress means higher chance of person feeling depressed.

### 17. Family History of Mental Illness

- No null value
- Looking at the graph, we can say that family history of mental illness does not really impact the person feeling depressed.

### 18. Target Variable - Depression
- No null value
- However, classes are imbalanced, more 0's than 1's. Therefore, for spliting the data we should use stratified sampling.


### Correlation matrix
- Depression has high correlation with almost all numeric columns except CGPA (noted before as well).
- Should check this graph again after data cleaning.
