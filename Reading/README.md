# Informedb-Internship-Report
## Problem 
This project will be looking at a legacy project called Informedb developed by Matt Child.  
"Informedb helps to identify and answer issues within a programs disparate datasets that will support sound engineering and technical decisions.  Understanding system of systems integration and coupling it with the other key challenges of a program’s tradeoff is critical in meeting the operational needs of any program." https://www.simventions.com/folio/informedb-enterprise/  
Software Quality Metrics are calculated to reflect the efficiency of preventing and removing defects.  

This project will be addressing the need for a comprehensize report on the quality of the informed-enterprise project

**Scope** 

I will be addressing the issue by mining all the data available on Jira for the Informedb Project on the company’s progress in finding issues, starting work on said issues, and resolving the issues. The project will require me to find eight different Software Quality Metrics:

* Direct Trends:  
This parameter measures the distribution of R1/R2/R3/R4 issues and measures what portion of the issues are one of those 4 options over the last year.

* Total Defects found in the last 4 weeks:  
Because this project is a legacy project, the lat four weeks do not have any recorded data. Because of this, the last four weeks of issues being reported will be counted.

* MTTR – Mean time to repair:  
This parameter is calculated by finding the mean of the repair time. Repair time should be calculated by

* Direct Removal Efficiency:  
DRE = (number of defects resolved/number of defects found externally and internally) * 100

* Number of failed fix attempts (external): 

* Number of failed fix attempts (internal):  

* Change failure rate within release cycle:  
The number of new defects introduced by a fix in your development cycle (sprint cycle); regression related. 

* Automated Code Coverage (in percent):  
Automated developmental tests provide a means of ensuring that updates to the code do not break previous functionality and that new functionality works as expected. Ideally, for each function that is implemented, a set of automated tests are constructed that cover both the specification for what the performance should achieve as well as the code that is used to implement that function.

All the data will be mined from GitHub and Jira, stored in an Excel file, and analyzed using RStudio, which will save my findings on a Word Document. This word document will be used for the final presentation.

**Constraints**

Some of the parameters above are going to be very difficult to extract. Without recording the number of times an issue was addressed, it would be very complicated to try to quantify these adjustments. Specifying whether these fixes are external or internal will be it's own challenge. Several metrics will be especially hard to find. Among these are Number of failed fix attempts, Change failure rate, and automated code coverage.

**All data is collected from the Informedb project on Jira. The project has assigned bug resolution data that was collected and organized to analyze with R.**   
  
This project is a product of Liam Whitenack's Summer Internship.  

## Problem Statement  



* Feasibility
* Viability
* Desireability
I will be addressing the issue by mining all the data available on Jira for the Informedb Project on the company’s progress in finding issues, starting work on said issues, and resolving the issues. The project will require me to find eight different Software Quality Metrics:  
•	Defect Trends  
•	Total Defects found in the last 4 weeks  
•	MTTR – Mean time to repair  
•	Defect Removal Efficiency  
•	Number of failed fix attempts (external)  
•	Number of failed fix attempts (internal)  
•	Change failure rate within release cycle  
•	Automated Code Coverage (in percent)  

•	Defects in four weeks- This column shows the number of defects over the last four weeks of issues being reported.  
•	MTTR (mean time to repair)- This column shows the average number of days spent from the creation of the project to the day it was last updated (only in cases where the status of the project is “Resolved”).
•	FFA (Failed Fix Attempts)- This column states the number of issues that have to be tested still.  
•	DRE (defect removal efficiency)- This column shows the number of total issues resolved divided by the number of total issues. 
•	Open- the number of projects that are left as "open"


Each parameter is found with the following method:  

* Defect Trends: This is reported as a histogram which reflects the number of bugs recorded in each period

* Defects in the last four weeks: In Jira, this would be calculated by counting the number of rows created in the last 28 days. Because this is a legacy project, the last 28 days of issues being created is used.
