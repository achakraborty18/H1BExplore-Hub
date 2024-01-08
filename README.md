# H1BExplore-Hub

## Overview

This is an initiative to identify companies providing H1B sponsorship to international employees. Utilizing governmental data over the past decade, the project focuses on analyzing the companies, skills, and job roles essential for improving the chances of obtaining H1B visa sponsorships. The envisaged API can be seamlessly integrated as an extension for platforms like LinkedIn, specifically within their "Job Search" section.

## Data Information

The data was extracted from the United States Department of Labor (DOL) website:  http://www.foreignlaborcert.doleta.gov/performancedata.cfm#dis

The dataset, comprising over 1.6 GB with 2+ million entries and 100 columns, covers various aspects of visa applications, categorized into 9 groups: case, job, employer, attorney/agent, website, wage, preparer, and others.

## Data Preprocessing

In the data preprocessing stage using Pandas, we streamlined the dataset by removing NULL and duplicate values, resulting in a reduction of records from 2,074,099 to 1,749,116. This process contributed to a size decrease from 1.6+ GB to 1.45 GB after the elimination of unnecessary columns.

## Backend (Relational database - SQL/PgAdmin/psycopg)

Transitioning to the backend, we configured databases specifically designed for housing H-1B data. This encompassed the incorporation of integrity constraints across 9 tables, ensuring the accuracy of the stored data. Furthermore, we crafted a query-generating function to retrieve filtered results based on user inputs.

## Frontend (Flask framework - HTML/CSS/Javascript/Python)

Designed within the Flask framework using HTML, CSS, Javascript, and Python, the user-friendly interface incorporates a dynamic search bar for inputs like job title, location, and company. Integrated filters further refine target roles based on parameters such as case status, time frame, pay, H-1B dependence, and employment type.

## API Page

![Screen Shot 2024-01-08 at 10 20 08 AM](https://github.com/achakraborty18/H1BExplore-Hub/assets/150084176/81981c5a-0c3e-4bb0-9c19-6cde3e75c8c7)

