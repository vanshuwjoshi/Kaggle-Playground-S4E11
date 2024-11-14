# Data Cleaning

### 1. Gender

- One-hot encoding since there is no ordinal relationship

### 2. Age

- Binning (Discretization) of Age
- group people into age ranges
- binning into an equal number of bins

### 3. City

- Cleaned the city column values
- Performed mean encoding for the city column

### 4. Working Professional or Student

- Binary column and we saw that student have high percentage of depressed people.
- Encoding 0-Working and 1-Student


### 5. Profession
- For the null values it could either be - Unemployed or Student
- 27800 are students. So can replace the null values with Student
- Rest null values = "Unemployed"
- People who have listed their wrong professions, are all working professionals, we can combine them together to "Others".
- Mean encoding


### 6. Academic Pressure and Work Pressure
- Combine Academic Pressure and Work Pressure as "Pressure"
- Rest of the null values are replaced by median = 3
- Drop the Academic Pressure


### 6. Study Satisfaction and Job Satisfaction
- Repeating the same as above


### 7. CGPA
- Filling null values with -1 (since the rows are for working professionals)
- Rest values are rounded.

### 8. Sleep Duration
- Created 4 categories - 5, 6, 7, 8. 
- More than 8 are 8, less than 5 are 5. If 1 hour range is provided = higher number. If more than 1 hour range provided = average
- If weekly provided - divide by 7
- Other incorrect values replaced by mode = 8.