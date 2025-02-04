# ISA616 Project 2: FSB Placement Data Insights

**Group #9: Linh Vu and Minh Mai**

## Project Overview

In the dynamic landscape of higher education, it's essential for academic institutions like the Farmer School of Business to stay informed about the outcomes of their graduates. Annually, the FSB conducts a senior survey of graduates to learn of their employment status. In addition, information is verified using LinkedIn and employer survey information. This project is driven by the need to understand the trends in student placement and salaries to evaluate the effectiveness of FSB's programs and guide future initiatives. The data ('FSB_BI_Survey_2019_2021.rds') contains data on graduates for 2019, 2020, and 2021. The data are merged from two sources: the senior survey, and data from the Miami University database.

This repository serves as the workspace for our second project in ISA 616, focusing on the analysis of FSB (Farmer School of Business) graduate placement data over the years 2019, 2020, and 2021.

## Client and Purpose

Our client for this project is Mr. Kirk Bogard, Associate Vice President for Development and External Relations at FSB. The data insights derived from this project will be utilized to achieve the following objectives:

1.  Inform Rankings: Utilize insights to enhance FSB's rankings.
2.  Support Admission Efforts: Provide factual data for prospective parents (Facts & Figures) and students (Fit & Feel) to make informed decisions about admission.
3.  Attract Corporate Partners: Showcase data to attract companies for recruiting FSB graduates.
4.  Influence Job Opportunities: Help influence the types of jobs and salary levels offered to FSB students.
5.  Brand Management: Strengthen FSB's brand with evidence-backed statements, such as "Farmer School students are job-ready on day one," supported by a top 10 ranking for Return on Investment (ROI).

Our analysis will provide valuable insights into the performance of FSB graduates in terms of placement and salary, aiding in informed decision-making and strategic planning for FSB.

## Key Data Points and Objectives

The primary purpose of our project is to address the following key questions:

1.  Placement Trends: We will analyze whether FSB's placement results have been on the rise, declining, or maintaining stability over the past three years. This analysis will provide valuable insights into the effectiveness of FSB in helping students secure jobs or job offers.

2.  Salary Trends: By examining salary trends, we will assess whether there have been changes in the earnings of FSB graduates. Understanding salary trends is crucial as it sheds light on the financial outcomes of our students.

3. Major-Specific Analysis: Our analysis goes beyond the overall trends. We will break down the data by specific majors to offer a detailed view of how placement and salary trends vary within different academic programs. This approach allows us to tailor strategies and investments in response to major-specific trends.

## Data Sources

We have three years of data representing FSB graduates, including graduates in 2019, 2020, and 2021. The dataset provided had 42 variables. The data has been meticulously compiled and cleaned, merging information from the senior survey and the Miami University database into one file.

1.  `nmajor`: numeric,derived, the number of majors
2.  `major1`: text, OBIEE, first major
3.  `major2`: text, OBIEE, second major
4.  `BBRJ`: binary, OBIEE, an attribute of a student, but we do not know what this stands for
5.  `Business Direct Admit`: binary, OBIEE, a direct admit to FSB as a first year
6.  `Combined Cacc and Masters`: binary, OBIEE, combined degree student
7.  `Dean's List`: binary, OBIEE, achieve dean's list status at least once
8.  `First Generation College Stdnt`: binary, OBIEE, first generation student status
9.  `FSB Scholars`: binary, OBIEE, FSB scholars program
10. `Honors Program`: binary, OBIEE, member of University honors program
11. `President's list`: binary, OBIEE, achieved president's list at least once
12. `Study Abroud Courtesy Account`: binary, OBIEE, do not know meaning
13. `Transfer Work`: binary, OBIEE, do not know exact meaning
14. `Cum Laude`: binary, OBIEE, graduated Cum Laude
15. `Magna Cum Laude`: binary, OBIEE, graduated Magna Cum Laude
16. `Summa Cum Laude`: binary, OBIEE, graduated Summa Cum Laude
17. `University Honors`: binary, OBIEE, graduated with University Honors
18. `University Honors w/Distinction`: binary, OBIEE, graduated with University Honors with Distinction
19. `minor1`: text, OBIEE, first listed minor
20. `minor2`: text, OBIEE, second listed minor
21. `IPEDS.Race.Ethnicity`: text, OBIEE, race/ethnicity
22. `Gender`: text, OBIEE, sex
23. `GPA.Range`: text, OBIEE, GPA within a .5 range
24. `Term.Code`: numberic, OBIEE, First four digits are the physcal year (beginning in July, e.g. July 2020 is FY 2021). Last two digits is the term (10=fall, 15=winter, 20=spring, 30=summer).
25. `Year.x`: text, derived, first four digits of Term.Code stored as a character variable
26. `latin_honors`: text, survey, latin honors designation
27. `survey_city`: text, survey, student reported city in which their job is located
28. `survey_company`: text, survey, student reported company in which they accepted a job
29. `survey_deptfunc`: text, survey, student reported job function
30. `survey_gradprogram`: text, survey, student reported graduate program they will be attending
31. `survey_gradschool`: text, survey, stuent reported graduate school they will be attending
32. `survey_internfour`: text, survey, student reported fourth internship they held during college
33. `survey_internthree`: text, survey, student reported third internship they held during college
34. `survey_interntwo`: text, survey, student reported second internship they held during college
35. `survey_internone`: text, survey, student reported first internship they held during college
36. `Survey_internships`: text, survey, Student reported number of internships they held during college
37. `survey_offers`: text, survey, student reported number of offers for full time employment received
38. `survey_plans`: text, survey, student reported plans after graduation
39. `survey_pref_field`: text, survey, student reported whether working in preferred field
40. `survey_pref_loc`: text, survey, student reported whether working in preferred location
41. `survey_salary`: numeric, survey, student reported salary
42. `survey_state`: text, survey, student reported state in which job is located

## Instructions

We recommend running the Student Success Project.Rmd first before the Student Success Dashboard. Rmd. This is because the first file reads in the original data survey and cleans it. The file also exports additional rds files for the second file to read in and use.  

## List of All Files

1. FSB_BI_Survey_2019_2021.rds: the original survey data file
2. Student Success Project.Rmd : our data cleaning and analysis file
3. kaggle-fortune500-1996-2023.csv : external dataset that we utilize in our analysis
4. Student Success Project.html : the data cleaning and analysis file knitted
5. Student Success Dashboard.Rmd : our dashboard that contains visualizations
6. Student Success Dashboard.html : our knitted dashboard
