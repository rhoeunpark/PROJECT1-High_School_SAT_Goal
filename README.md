# Problem Statement
In order for the high school students to adequately prepare for their admissions to  higher level education, it is important that they know what requirements that they should be achieving. This project aims to help the students establish a clear goal SAT score by exploring and comparing the SAT score trend across different colleges and majors.

# Background
Although many colleges are dropping standardized test requirement for admissions, 
standardized tests still serve as an important evaluation point in college admission process. For example, University of Pennsylvania which went test optional in 2020 due to Covid-19 pandemic reported that 75% of studnets who were accpeted early admission submitted test scores ([*source*](https://blog.prepscholar.com/do-you-have-to-take-the-sat). Having a score in hand also helps with the flexibility in coming up with a list of schools, as many schools still require, or will be back requiring a test score for admissions. Therefore, there is still worth in stressing the importance of having a good standardized test score in order to increase the chance of the students to get into the school and the field that they want.  

# Data

#### Datasets Used:
- 2019 SAT Scores by State (sat_2019.csv)
- 2019 SAT Scores by Intended College Major (sat_2019_by_intended_college_major.csv)
- Ranges of Accepted ACT & SAT Student Scores by Colleges (sat_act_by_college.csv)

#### Data Dictionary
|Feature|Type|Dataset|Description|
|---|---|---|---|
|**school**|*object*|scores_colleges|Name of the college/university where the information comes from.| 
|**test_optional**|*object*|scores_colleges|If the standardized test was optional for 2021 admission.|
|**for_class_year**|*object*|scores_colleges|In which years will the standardized test be optional for.| 
|**n_applicants**|*integer*|scores_colleges|Number of applicants to the given school.|
|**acceptance_rate**|*float*|scores_colleges|Percent accepted to the school out of the whole applicants.| 
|**sat_25th**|*float*|scores_colleges|25th percentile SAT score of the people accepted.| 
|**sat_75th**|*float*|scores_colleges|75th percentile SAT score of the people accepted.| 
|**sat_median**|*float*|scores_colleges|50th percentile/median score of the people accepted.| 
|**intended_college_major**|*object*|score-majors|Name of the major that the information directs to.| 
|**test_takers**|*integer*|score-majors|Number of test_takers who applied to the given major.| 
|**percent**|*float*|score-majors|Proportion of the applicants to the given major over the pool of applicants to all majors.| 
|**total**|*integer*|score-majors|Mean of total of reading, writing, math SAT scores| 
|**reading_writing**|*integer*|score-majors|Mean reading and writing score of the given major| 
|**math**|*integer*|score-majors|Mean math SAT score of the given major.| 
|**is_stem**|*boolean*|score-majors|Indicates whether the given major is considered STEM.| 
|**state**|*object*|state-sat-scores-2019|The name of the state in which the information belongs to.| 
|**participation_rate**|*float*|Proportion of the students of the states who participated in the SAT.| 
|**ebrw**|*integer*|state-sat-scores-2019|Mean reading and writing SAT score.| 
|**math**|*integer*|state-sat-scores-2019|Mean math SAT score.| 
|**total**|*integer*|state-sat-scores-2019|Mean SAT total score.| 

# Analysis
Average SAT score of California was slightly lower than the national average, which was calculated by averaging the scores of all states. 

Defining a student's 'safety schools' as schools in which the student's score is higher than the 75th percentile, the student with a score equal to CA's average score can consider 1 out of 410 schools as a safety school. 

The median scores for STEM majors are higher than that of the non-stem majors. The box plot also shows that the scores of STEM majors are aggregated around higher total scores. Referring to math only scores, the difference in median is similar to that of the total score; however, the scores of non-STEM majors are aggregated more towards the lower scores. 

There is a negative correlation between the school acceptance_rate vs sat_median of different colleges. Lower the acceptance rate, the median SAT scores of the accepted students tend to be higher. 

# Conclusions
----
#### In order for the high school students to adequately prepare for their admissions to  higher level education, it is important that they know what requirements that they should be achieving. This project aims to help the students establish a clear goal SAT score by exploring and comparing the SAT score trend across different colleges and majors.
----
Looking at the average SAT score of CA, there are many students who need to work toward higher SAT score if they aim to go to the colleges in the given list. Student who wish to enter as a STEM major need to aim for higher score, especially math. Using the acceptance rate as an indicator of prestigious school, students who aim to go to the prestigious schools also need to aim for higher SAT score.  
