# Emmanuel-s_Portfolio
#DATA ANALYST IN POWER-BI PROJECT 1:
##CASE STUDY; ANALYZING JOB MARKET DATA IN POWER BI

##Introduction:

I am a junior data analyst currently taking the data analyst in power bi career track with Datacamp, and this is my first project on the career track.

As my first project of power bi, I thought it was worth documenting to either serve as a note for future references or a learning tool for prospects. Come with me!

This job market data analysis focuses on investigating market trends for data science roles.


Context: An employee recruiting firm, Datasearch needs to uncover job trends in the data science roles.

Task: Discover trends in jobs and skills within the data science industry.

Data sets: A fictitious collection of crucial details from job postings from 2017 to 2021, each row correlates with a specific job posting in time and one table contains 19 columns.

Data source: I downloaded these datasets from my course overview on Datacamp. note: since the datasets are fictitious, they should not be applied to real-life scenarios.

For the sake of this project, I am using power bi, and this project would follow the data analysis pipeline with power bi which includes;

. Data check

. Data exploration

. Analysis and visualization

. Dashboards

. Communicating insights

I will start by importing and loading the datasets into my local power bi as a CSV file (comma-separated values).


The dataset contains (25,144 rows),

DATA CHECK AND EXPLORATION:

Investigating percentage of null values for minimum pay and maximum pay columns with power query.


Let's investigate columns with unique values.

changed column profiling from the top 1000 rows, to based on the entire dataset and selected column distribution under the view ribbon to display unique and distinct values for each column.

diving deeper into the columns, by looking at column statistics and column distribution, still on view ribbon, enabling column profile, and clicking on each column header further explores the details of each column.


Data column exploration
Exploring Trends In Job Postings Over Time:

Specifically looking at how the years of experience related to a particular position.

To understand the relationship between time and position level, I would visualize the average of Years of Experience required by each of the fields of Job position level and how the number of job postings changes over time.


Changes in job positions over time
Data Clean-Up to Specified Roles:

Datasearch has requested specific analysis of these job titles in Data science; Data scientist, Data analyst, Data engineer, Machine learning, and Data manager. Time to clean up some data!


The 5 roles of interest
Creating Some Calculated Columns With DAX:

To determine the minimum and maximum pay average, I used the data analytics expressions to create some calculated columns into a separate calculations table.


Average pay calculated column from max_pay and min_pay

Average of average pay calculated column
Effect of years of experience on salary:

I am investigating what is influencing job market trends. for this, I looked at different roles’ salaries and how they change with years of experience.


Effect of years of experience on salaries
ANALYSIS AND VISUALIZATION:

Let's jump into analyzing the job skills column, this column contains values in a list.


List of job skills
I need to clean this up to proceed with further analysis.


Job Skills cleaned up
Job skills are cleaned up, split into rows, and ready for analysis.

I created a visualization showing the count of all the different skills.


Likelihood of skills in job postings:

I used the power of DAX to better understand what is the percentage chance that a certain skill will be listed in a job posting by creating the job posting count measure, skill count measure, and the percentage of skills on each posting.

DAX measures
DAX
And creating a matrix showing the likelihood that a certain skill will be listed in a job posting.


r
I also added a slicer to the visual for ease of accessing the information on a skill of choice.

Analyzing Trends In Skills Over Time:

It is also necessary to explore how skills in job postings trend over time, to archive this I would have to put my new measure to good use.


The trend in skills over time
Deep dive into five (5) key job analyses:

I needed to explore better the top companies and industries looking for data science roles. To get this done I further analyzed the data by visualizing using the following columns;

[years of experience (avg. years of experience )]

[company industry]

[company size] and

[job skills]


five (5) key job analysis
After a thorough analysis of the five (5) key job titles that datasearch suggested, there are other job titles that I could consider and recommend for datasearch that has similar experience requirements.


other titles and skills required
this is a distribution of the top 20 job titles with similar skill requirements.

DASHBOARDS AND INSIGHTS:

In this segment, I will be focusing on building a dashboard for datasearch.

There are a few questions to ask before I proceed with this dashboard,

Who
What
How
.Who is the audience? Datasearch.

.What do they need? Identify optical opportunities and present the right jobs to qualified candidates.

.How can the dashboard help? The dashboard needs to be more than just exciting visuals, it has to be created with the client’s goal in mind to help them solve problems in a particular manner.

Before building these dashboards I included some of the job titles I recommended for datasearch that has similar skill and experience requirements.

HOME PAGE;

The job, skills, and company icons on the home page are interactive, they are links to the respective dashboards.


Home Page
Jobs Dashboard;

This is an overview of the job visuals which include; Job skills by job title, Average years of experience by job position, job posting by year and position level, number of job postings, and average year of experience.


Jobs dashboard
Skills Dashboard;

An overview of the skills putting together a visual analysis from the percentage of job postings by year, distribution of job skills count across different skills, skills count, and job postings counts.


Skills dashboard
Company dashboard;

The company overview includes a visual analysis of the company industry by job position and avg_year of experience, company industry by job posting and avg_year of experience, company industry by the count of job skills, and a table showing company name, job title, and posting count, and a gauge showing avg_pay, avg_minimum pay, and Avg_maximum pay.


Company dashboard
I am ready to learn, open to corrections, and looking forward to my first internship. Thank you!

connect with me on Linkedin https://bit.ly/3QkJWHv

26


2


26


2




More from Emmanuel Onu
Data analyst
