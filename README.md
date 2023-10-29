## Overview of the Repository

This repository will hold our data and updates for the FSB Placement Data Insights project - ISA 616. 
The collaborators on this project are Brady Stultz and Ellie Hoog.

## Project Overview

Annually, the FSB conducts a senior survey of graduates to learn of their employment status.  In addition, information is verified using LinkedIn and employer survey information.  The data you are provided ('FSB_BI_Survey_2019_2021.rds') contains data on graduates for 2019, 2020, and 2021.  The data are merged from two sources:  the senior survey, and data from the Miami University database.  

The data are anonymized, however it is possible that if you look hard enough, you can identify students.  You are bound, ethically not to do so.  It is a strict ethical code that you will not discuss individual data points with ANYONE except for me and your team.  Failure to comply with this code of ethics will result in a failing grade in the course.  

## Project Goals

For this project, we will examine the correlation between internships and full-time placement. More specifically, we will answer the following questions:
1. If a student has at least one internship, how much more likely are they to have a full-time job than if they did not have an internship?
2. What if a student has two internships?
3. Does having an internship mean your salary level will be higher in your full-time job?

From our team's personal experience, we have found that there is immense pressure on students to secure at least one internship during their time at Miami. We are hoping our insights will shed more light on the subject using a data-centric approach. 

## Project Statement

This project, including its data and visualizations, will inform our client (and subsequent audiences) about the relationship between internships and full-time placement after graduation. With our findings, we aim to aid our client in promoting FSB to companies of interest and strengthening external relationships.

## Deliverables

Student Success Dashboard: a collection of data visualizations for our client that can be presented to potential companies in search of a partnership with FSB, or families of prospective students looking to see the benefits of FSB regarding internships and full-time placement after graduation. This dashboard will relieve the pain of attracting recruiters to obtain talent fom Miami based on student interest. Our findings can optimize the allocation of resources to different majors and years in the internship search.

## Data Sources

You have three years of data representing FSB graduates, including graduates in 2019, 2020, and 2021.  The dataset provided had 42 variables.  The source is either derived by me during data cleaning/merging, from the Oracle Business Intelligence Enterprise Edition (OBIEE) maintained by Miami adminsitration, or from the self reported senior survey.  I have cleaned and merged the files into one file.  

1.  nmajor: numeric,derived, the number of majors 
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

## Contents of Github Folder

1. .gitignore: Allows the data to not be committed (we are working with a public repository).
2. Analytics Class Project from Client.docx: Outline of project from client
3. cleandata.RDS: Clean data file
4. FSB_BI_Survey_2019_2021.rds: Original data file
5. ISA616-CareerProj.Rproj: R project where our work was conducted
6. README.md: Provides an overview of our project to the client
7. Student Success doc.Rmd/html: Overview of project, Business Value Proposition, data pre-processing
8. StudentSuccessDashboard.Rmd/html: Final dashboard visualization of our findings
9. Student Success - Github Link: link to our public Github repository
