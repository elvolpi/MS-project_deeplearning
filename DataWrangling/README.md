We have two models, one for lower division courses and one for student and terms data. 

Our data :
- student is entering demographic information about the student 97555 rows x 13 columns.
- term: contains information on standing, GPA, credit hours, and any
changes in major 639,915 x 13 
- course: contains every course the student has taken (grade, class
number, section, level) 3289532 x 13 columns

Goals of data wrangling 
- Remove NA's 
  - Keras cannot handle any NA's
  - Keras will not tell you if you have NA’s
  - We experienced non-relevant errors, loss of NA and computer
crashing/high RAM usage instead

- Make all data numeric 
  - once again for Keras functionality 
  - Encode characters
  - Standardize nominal variables: results in the best loss

- Need to get all data on the student level, ”widening” the data so
each row represents one distinct student
- Make variable decisions as to not overfit or give highly correlated
explanatory variables




