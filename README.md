# Jira Issue Analyzer

This code was made to calculate metrics that were requested by the Military. These Metrics are listed in the "NSWCCD_Software_Quality_Metrics.pdf" file attached. In addition to calculating these Software Quality Metrics, this code performs an analysis that allows the user to take a close look at the data from Jira.  

### Dataframe Files
* "Informedb Jira Data.csv" is the file containing all of the data exported from Jira, pertaining to Informedb.  
* "Informedb_NSWCCD_data.csv" is the cleaned file that contains the Informedb bugs and uses the military's terms.  
* "Informedb_Reliability_Metrics" is the file that contains the computed software quality metrics requested for Informedb.  
* "Informedb_tidy" is the cleaned file for Informedb Jira Data.  

### Markdown Files
* "Jira_Issues_Analysis.Rmd" Is a file that performs an analysis of Jira data using Shiny that allows the user to look closely on the entire history of Informedb.  
* "Jira_Project_Data_Rebuild" Is a file that takes the raw data from a Jira Export and outputs reliability metrics and a tidied file that allows further analysis.  
* "NSWCCD_Metrics_Analysis.Rmd" Is the file used to present research on software quality metrics for Informedb. It uses the military terms and only examines defects. 

### How to use this file for new projects
To run this code, R and RStudio must both be downloaded. GitHub projects can be opened in RStudio by Clicking "New Project" on the top right,
1. First, output data from Jira. In order to retrieve Jira Data, go to Issues -> View all issues and filters -> Export -> CSV (All fields). Rename the file to something you can remember.  
2. Open "Jira_Project_Data_Rebuild.Rmd" and replace the .csv file on line 46 with the newly made .csv file. Change "Informedb" to the name of your project on line 440 and 442. 
3. To perform an analysis of the Issues on Jira, go to "Jira_issues_Analysis.Rmd" and change the name of the file to "(your project name)_tidy.csv"
