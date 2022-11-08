# DATA ANALYST IN POWER-BI PROJECT

## CASE STUDY; ANALYZING JOB MARKET DATA IN POWER-BI

## Introduction:

I am a junior data analyst currently taking the data analyst in Power-Bi career track with [Datacamp](datacamp.com), and this is my first project on the career track.

As my first project of Power-Bi, I thought it was worth documenting to either serve as a note for future references or a learning tool for prospects. Come with me!

This job market data analysis focuses on investigating market trends for data science roles.

![job market img](https://user-images.githubusercontent.com/106547277/200588896-3f48bd49-e270-4eef-bb21-c457c14f3fe2.jpg)

#### Context: 
An employee recruiting firm, Datasearch needs to uncover job trends in the data science roles.

#### Task: 
Discover trends in jobs and skills within the data science industry.

#### Data sets: 
A fictitious collection of crucial details from job postings from 2017 to 2021, each row correlates with a specific job posting in time and one table contains 19 columns.

#### Data source: 
I downloaded these datasets from my course overview on [Datacamp](datacamp.com). note: since the datasets are fictitious, they should not be applied to real-life scenarios.

For the sake of this project, I am using Power-Bi, and this project would follow the data analysis pipeline with Power-Bi which includes;

. Data check

. Data exploration

. Analysis and visualization

. Dashboards

. Communicating insights

I will start by importing and loading the datasets into my local Power-Bi as a CSV file (comma-separated values).

![Screenshot 2022-05-20 040752](https://user-images.githubusercontent.com/106547277/200590456-ea9f52d7-5e42-41cb-8d0e-74645cc0ca01.png)

The dataset contains (25,144 rows),

## DATA CHECK AND EXPLORATION:

Investigating percentage of null values for minimum pay and maximum pay columns with power query.

![Screenshot 2022-05-20 044726_LI](https://user-images.githubusercontent.com/106547277/200590899-042196f6-dca2-4fb4-bd92-cc20e5789416.jpg)



#### Let's investigate columns with unique values.


changed column profiling from the top 1000 rows, to based on the entire dataset and selected column distribution under the view ribbon to display unique and distinct values for each column.

diving deeper into the columns, by looking at column statistics and column distribution, still on view ribbon, enabling column profile, and clicking on each column header further explores the details of each column.

![data check column investigations](https://user-images.githubusercontent.com/106547277/200591713-c2188618-4eba-40e2-b022-02ea2c90e43e.png)

Data column exploration


#### Exploring Trends In Job Postings Over Time:

Specifically looking at how the years of experience related to a particular position.

To understand the relationship between time and position level, I would visualize the average of Years of Experience required by each of the fields of Job position level and how the number of job postings changes over time.

![changes in job positions over time](https://user-images.githubusercontent.com/106547277/200592237-058a7326-8899-49d8-982d-65008312922f.png)

Changes in job positions over time



#### Data Clean-Up to Specified Roles:

Datasearch has requested specific analysis of these job titles in Data science; Data scientist, Data analyst, Data engineer, Machine learning, and Data manager. Time to clean up some data!

![5 jobs of interest](https://user-images.githubusercontent.com/106547277/200592665-de1b0288-c8d0-4b0e-ad37-784b03431a34.png)

The 5 roles of interest




#### Creating Some Calculated Columns With DAX:

To determine the minimum and maximum pay average, I used the data analytics expressions to create some calculated columns into a separate calculations table.

![Average pay calculated column](https://user-images.githubusercontent.com/106547277/200593675-702c137f-95dd-490e-bc16-0f781b530ce9.png)

Average pay calculated column from max_pay and min_pay



![calculated column 2](https://user-images.githubusercontent.com/106547277/200594021-9d8a4307-5e86-4d05-99ab-fb11399926bf.png)

Average of average pay calculated column


#### Effect of years of experience on salary:

I am investigating what is influencing job market trends. for this, I looked at different roles’ salaries and how they change with years of experience.

![Average pay by year of experience and job title](https://user-images.githubusercontent.com/106547277/200594768-f9e51a94-b83b-46f1-880c-c1551b088f18.png)

Effect of years of experience on salaries


## ANALYSIS AND VISUALIZATION:

Let's jump into analyzing the job skills column, this column contains values in a list.

![job skills clean up](https://user-images.githubusercontent.com/106547277/200597839-72773fc1-4974-4ac3-a6c7-3852db2ceafa.png)

List of job skills
I need to clean this up to proceed with further analysis.

![cleaned job skills](https://user-images.githubusercontent.com/106547277/200598186-855022d8-8459-4739-9e0e-432e298b4bf6.png)

Job Skills cleaned up

Job skills are cleaned up, split into rows, and ready for analysis.

I created a visual showing the count of all the different skills.

![count of job skills by job skills](https://user-images.githubusercontent.com/106547277/200598387-4b940701-d025-4372-828b-d3e7498e76ad.png)

Likelihood of skills in job postings:



I used the power of DAX to better understand what is the percentage chance that a certain skill will be listed in a job posting by creating the job posting count measure, skill count measure, and the percentage of skills on each posting.

![likelihood of skill DAX](https://user-images.githubusercontent.com/106547277/200598997-eaf4fe01-14c7-4ee8-840b-7bb8c3d95f98.png)

DAX measures


And creating a matrix showing the likelihood that a certain skill will be listed in a job posting.

![Likelihood visual cleaned up](https://user-images.githubusercontent.com/106547277/200599452-91c6cff7-8844-4937-9735-c3bf8f1d8d24.png)


I also added a slicer to the visual for ease of accessing the information on a skill of choice.

## Analyzing Trends In Skills Over Time:

It is also necessary to explore how skills in job postings trend over time, to archive this I would have to put my new measure to good use.

![trend in skills over time](https://user-images.githubusercontent.com/106547277/200599914-edb4efa5-ce66-4bc2-b3d8-489cfe375ecb.png)

The trend in skills over time


#### Deep dive into the five (5) key job analyses:

I needed to explore better the top companies and industries looking for data science roles. To get this done I further analyzed the data by visualizing using the following columns;

[years of experience (avg. years of experience )]

[company industry]

[company size] and

[job skills]

![key job descriptions](https://user-images.githubusercontent.com/106547277/200600167-458cd8a9-55c7-4bf0-968b-c7f130943358.png)

five (5) key job analysis

After a thorough analysis of the five (5) key job titles that datasearch suggested, there are other job titles that I could consider and recommend for datasearch that has similar experience requirements.

![similar job titles](https://user-images.githubusercontent.com/106547277/200600717-b033c76a-ff03-449a-b01d-45ddf8604794.png)

other titles and skills required

this is a distribution of the top 20 job titles with similar skill requirements.

## DASHBOARDS AND INSIGHTS:

In this segment, I will be focusing on building a dashboard for datasearch.

There are a few questions to ask before I proceed with this dashboard,

Who
What
How
.Who is the audience? Datasearch.

.What do they need? Identify optical opportunities and present the right jobs to qualified candidates.

.How can the dashboard help? The dashboard needs to be more than just exciting visuals, it has to be created with the client’s goal in mind to help them solve problems in a particular manner.

Before building these dashboards I included some of the job titles I recommended for datasearch that has similar skill and experience requirements.

## HOME PAGE;

The job, skills, and company icons on the home page are interactive, they are links to the respective dashboards.

![Home page](https://user-images.githubusercontent.com/106547277/200601015-59e5b1c6-edcf-4678-baef-34a9d24b8d03.png)

Home Page


## Jobs Dashboard;

This is an overview of the job visuals which include; Job skills by job title, Average years of experience by job position, job posting by year and position level, number of job postings, and average year of experience.

![jobs page](https://user-images.githubusercontent.com/106547277/200601311-c9941205-8a4b-482b-9ccd-0d378a6aa513.png)

Jobs Dashboard


## Skills Dashboard;

An overview of the skills putting together a visual analysis from the percentage of job postings by year, distribution of job skills count across different skills, skills count, and job postings counts.

![skills page](https://user-images.githubusercontent.com/106547277/200601553-da8ff3ca-ea5b-49bc-b8fa-49e3c899d97d.png)

Skills dashboard


## Company dashboard;

The company overview includes a visual analysis of the company industry by job position and avg_year of experience, company industry by job posting and avg_year of experience, company industry by the count of job skills, and a table showing company name, job title, and posting count, and a gauge showing avg_pay, avg_minimum pay, and Avg_maximum pay.

![Company overview](https://user-images.githubusercontent.com/106547277/200602012-bdaf32e5-1bde-4d6e-b249-e6c6bc7f7f7b.png)

Company dashboard

[Click here](https://app.powerbi.com/groups/me/reports/62624842-b23f-4ef3-9ef4-b91420b8e6fc) to view project on Power-Bi service

I am ready to learn, and open to corrections. Thank you!

[Click here](https://www.linkedin.com/in/emmanuel-onu-287691165?lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_view_base_contact_details%3BRvOty7KAQ%2B6gxy3WjazJXg%3D%3D) to connect with me on Linkedin





More from Emmanuel Onu
Data analyst
