Brendan Beattie and Jake Holroyd
Group 18

# Project Overview

In this project, we plan to deliver insights and provide recommendations on student placement and salary trends from the Farmer School of Business to Kirk Bogard and the wonderful people at the FSB careers center. Our goal is to give the careers center the tools they need to best advise students who are seeking answers to their employment questions and concerns. We plan to do this by creating a time series analysis and visualizations to easily show the changing trends in how FSB students are being recruited in the job market as a whole and by major. Our two key metrics will be the results of placement data and salary trends that have been reported by recently hired graduates. Our solution will give the careers center the information they need to accurately inform students about what to expect in the placement process and what to seek as fair compensation based on how students from their major have performed in recent years. This solution will also give the careers center insight into what types of students may need extra help in the placement process and provide assistance to position students for the most success possible. 

## Data Context

Annually, the FSB conducts a senior survey of graduates to learn of their employment status.  In addition, information is verified using LinkedIn and employer survey information.  The data you are provided ('FSB_BI_Survey_2019_2021.rds') contains data on graduates for 2019, 2020, and 2021.  The data are merged from two sources:  the senior survey, and data from the Miami University database.  

The data are anonymized, however it is possible that if we look hard enough, we can identify students.  We are bound, ethically not to do so.  It is a strict ethical code that we will not discuss individual data points with ANYONE except for Dr. Farmer and our team.  Failure to comply with this code of ethics will result in a failing grade in the course.  

## Data Sources

We have been given three years of data representing FSB graduates, including graduates in 2019, 2020, and 2021.  The dataset provided had 42 variables.  The source is either derived by Dr. Farmer during data cleaning/merging, from the Oracle Business Intelligence Enterprise Edition (OBIEE) maintained by Miami adminsitration, or from the self reported senior survey.  Dr. Farmer has cleaned and merged the files into one file.  

## Files Table of Contents

- [Analytics Class Project From Client](#Analytics Class Project From Client)
- [Dashboard Markdown](#Dashboard.Rmd)
- [Dashboard Output](#Dashboard.html)
- [FSB Data Analysis Markdown](#FSBDataAnalysis.Rmd)
- [FSB Data Analysis Output](#FSBDataAnalysis.html)
- [Cleaned Data File](#FSB_job.csv)
- [R Project Directory](#ISA616-CareerProj.Rproj)

## Analytics Class Project From Client

This document summarizes the clients points of interest for our analysis.
- We chose to investigate the problem posed in prompt #4 regarding job placement and salary rates at FSB.

## Dashboard Markdown

This document is the markdown code file that constructs the final output of visualizations used in our analysis. The graphs created here are displayed in the final output.

## Dashboard Output

This document is a knitted .html file that is specially created to display the visualizations necessary for our analysis and conclusions (which are also displayed on the first page of the dashboard).

## FSB Data Analysis Markdown

This document is the markdown code file that follows our process of analysis, from defining our question, explaining of our business value proposition, and showing our work on the final cleaning and preparation of the data.

- Research Question 
- Business Value Proposition
 - Visualization
 - Text
- The Data
 - Data Sources 
 - Data Cleaning
  - Exploring Context
  - Counting Missing by Variable
  - Cleaning Non-standard responses
  - Imputation
 - Session Information

## Features

[List of features...]

## Contributing

[Contribution guidelines...]

## License

[License information...]

## FSB Data Analysis Output

This document is a knitted .html file output of the Markdown analysis document and is intended as a more accessible and digestible view of our process.

## Cleaned Data File

This document is a .csv file that contains the final, cleaned dataset developed in the FSB Data Analysis Markdown and is loaded in to be used for the visualizations in the Dashboard Markdown and corresponding Output.

## R Project Directory

This is the project directory file we used during the development of this analysis.

## Data Sources

We have been given three years of data representing FSB graduates, including graduates in 2019, 2020, and 2021.  The dataset provided had 42 variables.  The source is either derived by Dr. Farmer during data cleaning/merging, from the Oracle Business Intelligence Enterprise Edition (OBIEE) maintained by Miami adminsitration, or from the self reported senior survey.  Dr. Farmer has cleaned and merged the files into one file.

1.  major: numeric,derived, the number of majors 
2.  major1: text, OBIEE, first major
3.  major 2: text, OBIEE, second major
4.  BBRJ: binary, OBIEE, an attribute of a student, but we do not know what this stands for
5.  Business Direct Admit: binary, OBIEE, a direct admit to FSB as a first year
6.  Combined Cacc and Masters: binary, OBIEE, combined degree student
7.  Dean's List: binary, OBIEE, achieve dean's list status at least once
8.  First Generation College Stdnt: binary, OBIEE, first generation student status
9.  FSB Scholars: binary, OBIEE, FSB scholars program
10.  Honors Program: binary, OBIEE, member of University honors program
11.  President's list: binary, OBIEE, achieved president's list at least once
12.  Study Abroud Courtesy Account: binary, OBIEE, do not know meaning
13.  Transfer Work: binary, OBIEE, do not know exact meaning
14.  Cum Laude: binary, OBIEE, graduated Cum Laude
15.  Magna Cum Laude: binary, OBIEE, graduated Magna Cum Laude
16.  Summa Cum Laude: binary, OBIEE, graduated Summa Cum Laude
17.  University Honors: binary, OBIEE, graduated with University Honors
18.  University Honors w/Distinction: binary, OBIEE, graduated with University Honors with Distinction
19.  minor1: text, OBIEE, first listed minor
20.  minor2: text, OBIEE, second listed minor
21.  IPEDS.Race.Ethnicity: text, OBIEE, race/ethnicity
22.  Gender: text, OBIEE, sex
23.  GPA.Range: text, OBIEE, GPA within a .5 range
24.  Term.Code: numberic, OBIEE, First four digits are the physcal year (beginning in July, e.g. July 2020 is FY 2021).  Last two digits is the term (10=fall, 15=winter, 20=spring, 30=summer).
25.  Year.x: text, derived, first four digits of Term.Code stored as a character variable
26.  latin_honors: text, survey, latin honors designation
27.  survey_city: text, survey, student reported city in which their job is located
28.  survey_company: text, survey, student reported company in which they accepted a job
29.  survey_deptfunc: text, survey, student reported job function
30.  survey_gradprogram: text, survey, student reported graduate program they will be attending
31.  survey_gradschool: text, survey, stuent reported graduate school they will be attending
32.  survey_internfour: text, survey, student reported fourth internship they held during college
33.  survey_internthree: text, survey, student reported third internship they held during college
34.  survey_interntwo: text, survey, student reported second internship they held during college
35.  survey_internone: text, survey, student reported first internship they held during college
36.  Survey_internships: text, survey, Student reported number of internships they held during college
37.  survey_offers: text, survey, student reported number of offers for full time employment received
38.  survey_plans: text, survey, student reported plans after graduation
39.  survey_pref_field: text, survey, student reported whether working in preferred field
40.  survey_pref_loc: text, survey, student reported whether working in preferred location
41.  survey_salary: numeric, survey, student reported salary
42.  survey_state: text, survey, student reported state in which job is located

