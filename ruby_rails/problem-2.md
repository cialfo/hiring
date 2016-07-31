Problem 2
===
##### Find Super Score

The table below shows SAT test score of a student who has given the test 5 times

| math_score | reading_score | writing_score | test_date | 
| -------    | ----------    | ------------- | ------------- |
| 750	     | 650           | 650	          | 2016-01-01 00:00:00 | 
| 740	     | 610           | 680	          | 2016-02-01 00:00:00 | 
| 790	     | 450           | 750	          | 2016-03-01 00:00:00 | 
| 800	     | 600           | 700	          | 2016-04-01 00:00:00 | 
| 770	     | 690           | 710	          | 2016-05-01 00:00:00 |


Write a ruby program to find super score of the SAT test. A super score is the sum of maximum of each section (maths, reading, writing) from all the tests given so far.

So for the above example, the super score would be 800 (maths) + 690 (reading) + 750 (writing) = 2240.

**Input**

Take number of tests (n) and then data as row of inputs with space separated values

Example:   
3   
750 650 650 2016-01-01 00:00:00   
740 610 680 2016-02-01 00:00:00   
790 450 750 2016-03-01 00:00:00   

**output**

Individual max score and the super score in the next line

Example:   
790, 650, 750   
2190

