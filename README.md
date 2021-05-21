# Informedb-Internship-Report
**Problem** 

The issue I will be addressing will be the military’s request for organized and presented data on projects.  

 

**Scope** 

I will be addressing the issue by mining all the data available on Jira and GitHub for the Informedb Project on the company’s progress in finding issues, starting work on said issues, and resolving the issues. The project will require me to find eight different Software Quality Metrics:


* Total Defects found in the last 4 weeks:  
The issues for this project have not been updated since the company went online. I do not have the last 4 weeks of total defects. However, I can measure the amount of defects detected in 4-week spans, including the last 4 weeks of recorded data.

* Direct Trends:  
This parameter measures the distribution of R1/R2/R3/R4/R5 issues and measures what portion of the issues are one of those 5 options.

* MTTR – Mean time to repair:  
This parameter is the simplest one to implement: measured in hours, what is the time difference of when the issue was reported and when the issue was resolved. Many of the issues were never resolved. These issues will be recorded separately and the time between the last update and the start of the project will be recorded.

* Direct Removal Efficiency:  
DRE = (number of defects resolved/number of defects found externally and internally) * 100

* Number of failed fix attempts (external):  

* Number of failed fix attempts (internal):  

* Change failure rate within release cycle:  
The number of new defects introduced by a fix in your development cycle (sprint cycle); regression related. 

* Automated Code Coverage (in percent):  
Automated developmental tests provide a means of ensuring that 
updates to the code do not break previous functionality and that new 
functionality works as expected. Ideally, for each function that is 
implemented, a set of automated tests are constructed that cover both 
the specification for what the performance should achieve as well as the 
code that is used to implement that function.

All the data will be mined from GitHub and Jira, stored in an Excel file, and analyzed using RStudio, which will save my findings on a Word Document. This word document will be used for the final presentation.

**Constraints**

Some of the parameters above are going to be very difficult to extract. Without recording the number of times an issue was addressed, it would be very complicated to try to quantify these adjustments. Specifying whether these fixes are external or internal will be it's own challenge. 
