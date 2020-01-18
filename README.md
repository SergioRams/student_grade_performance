### Two Portuguese schools student performance regression problem.

This a student performance regression problem. In this repo you can find data visualization, multiple training model 
using cross validation techniques and test predictions. 

## Data Set Information:  

This data approach student achievement in secondary education of two Portuguese schools. The data attributes include 
student grades, demographic, social and school related features) and it was collected by using school reports and 
questionnaires. Two datasets are provided regarding the performance in two distinct subjects: Mathematics (mat) and 
Portuguese language (por).

Important note: the target attribute G3 has a strong correlation with attributes G2 and G1. This occurs because G3 is 
the final year grade (issued at the 3rd period), while G1 and G2 correspond to the 1st and 2nd period grades. It is more
 difficult to predict G3 without G2 and G1, but such prediction is much more useful (see paper source for more details).

###### Original dataset from: https://archive.ics.uci.edu/ml/datasets/student+performance

##### Attributes for both student-mat.csv (Math course) and student-por.csv (Portuguese language course) datasets:

<ol>
<li>school - student's school (binary: 'GP' - Gabriel Pereira or 'MS' - Mousinho da Silveira)</li>  
<li>sex - student's sex (binary: 'F' - female or 'M' - male)</li>
<li>age - student's age (numeric: from 15 to 22)</li>
<li>address - student's home address type (binary: 'U' - urban or 'R' - rural)</li>
<li>famsize - family size (binary: 'LE3' - less or equal to 3 or 'GT3' - greater than 3)</li>
<li>Pstatus - parent's cohabitation status (binary: 'T' - living together or 'A' - apart)</li>
<li>Medu - mother's education (numeric: 0 - none, 1 - primary education (4th grade), 2 â€“ 5th to 9th grade, 3 â€“ secondary education or 4 â€“ higher education)</li>
<li>Fedu - father's education (numeric: 0 - none, 1 - primary education (4th grade), 2 â€“ 5th to 9th grade, 3 â€“ secondary education or 4 â€“ higher education)</li>
<li>Mjob - mother's job (nominal: 'teacher', 'health' care related, civil 'services' (e.g. administrative or police), 'at_home' or 'other')</li>
<li>Fjob - father's job (nominal: 'teacher', 'health' care related, civil 'services' (e.g. administrative or police), 'at_home' or 'other')</li>
<li>reason - reason to choose this school (nominal: close to 'home', school 'reputation', 'course' preference or 'other')</li>
<li>guardian - student's guardian (nominal: 'mother', 'father' or 'other')</li>
<li>traveltime - home to school travel time (numeric: 1 - <15 min., 2 - 15 to 30 min., 3 - 30 min. to 1 hour, or 4 - >1 hour)</li>
<li>studytime - weekly study time (numeric: 1 - <2 hours, 2 - 2 to 5 hours, 3 - 5 to 10 hours, or 4 - >10 hours)</li>
<li>failures - number of past class failures (numeric: n if 1<=n<3, else 4)</li>
<li>schoolsup - extra educational support (binary: yes or no)</li>
<li>famsup - family educational support (binary: yes or no)</li>
<li>paid - extra paid classes within the course subject (Math or Portuguese) (binary: yes or no)</li>
<li>activities - extra-curricular activities (binary: yes or no)</li>
<li>nursery - attended nursery school (binary: yes or no)</li>
<li>higher - wants to take higher education (binary: yes or no)</li>
<li>internet - Internet access at home (binary: yes or no)</li>
<li>romantic - with a romantic relationship (binary: yes or no)</li>
<li>famrel - quality of family relationships (numeric: from 1 - very bad to 5 - excellent)</li>
<li>freetime - free time after school (numeric: from 1 - very low to 5 - very high)</li>
<li>goout - going out with friends (numeric: from 1 - very low to 5 - very high)</li>
<li>Dalc - workday alcohol consumption (numeric: from 1 - very low to 5 - very high)</li>
<li>Walc - weekend alcohol consumption (numeric: from 1 - very low to 5 - very high)</li>
<li>health - current health status (numeric: from 1 - very bad to 5 - very good)</li>
<li>absences - number of school absences (numeric: from 0 to 93)</li>
</ol>

#####  These grades are related with the course subject, Math or Portuguese:

<ul>
<li>31. G1 - first period grade (numeric: from 0 to 20)</li>
<li>31. G2 - second period grade (numeric: from 0 to 20)</li>
<li>32. G3 - final grade (numeric: from 0 to 20, output target)</li>
</ul>
