# Using a decision tree to predict if someone will get hired

Just a bit of fun, but a subject close to my heart since I’ve been looking for work the last few months without success. I’m not even talking about getting job offers, I mean I can’t even get an interview. Hmmm …. wonder why?

Decision trees and their use is one of the easier concepts in data science for people to get their heads around. It comes down to selecting an output based on a series of inputs – much like a series of nested IF-THEN-ELSE statements in a programming language.

The example shows what the likely hood of getting a job based on certain criteria. The input data is shown below.

```
Years Experience|Age|Employed?|Previous employers |Level of Education |Hired
----------------|---|---------|-------------------|-------------------|-----
25	        |56 |N	      |4                  |BSc	              |N
0	        |26 |Y	      |0	          |BSc	              |Y
28	        |55 |N	      |1	          |MSc	              |N
2	        |30 |Y	      |1	          |MSc	              |Y
20	        |49 |N	      |2	          |PhD	              |N
0	        |20 |Y	      |0	          |PhD	              |Y
5	        |27 |Y	      |2	          |MSc	              |Y
3	        |29 |Y	      |1	          |BSc	              |Y
22	        |53 |Y	      |5	          |BSc	              |N
0	        |19 |Y	      |0	          |BSc	              |Y
1	        |21 |Y	      |1	          |PhD	              |Y
4	        |26 |Y	      |1	          |BS	              |Y
0	        |20 |Y	      |0	          |PhD	              |Y
```

So we’re trying to predict whether a person will get a job based on their age, experience, education level and number of previous employers. The attached jupyter/python notebook will demonstrate the use of decision trees using the above dataset, scikitlearn and some basic numpy/panda/dataframe operations to predict the likely hood of a person getting hired.
