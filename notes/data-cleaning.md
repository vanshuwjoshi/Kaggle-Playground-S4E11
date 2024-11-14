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