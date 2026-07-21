# data-professional-survey-dashboard
This is a Power BI fsdjnpsrd I build using a real survey of 630 people who work in data jobs ( Data Analyst, Data Scientist, Data Engineer, and more). 
I made this project to practice my power BI skills and to show what I can do. 

# Why I made this 
I wanted to answer some real questions about working in data:

* Which job title pays the most?
* Are people happy wit their salary and work/life balance?
* What programming language do most people use?
* Is there a salary difference between men and woman?

# About the data
The data comes from a survey with 630 answers. It has information like job title, salary, industry, favorite programming language, happiness scores (0 to 10), country, age, gender, and education.	


# Toots I used 
* Power Query to clean the data
* Power BI to build the dashboard
* DAX to write formulas and calculations

# How I cleaned the data
The raw data was messy, so before building anything I had to:

* Remove empty columns I didn't need, like browser and city
* Change the salary from text ("106k-125k") into a real number, so I could calculate averages
* Fix messy answers like "Other (Please Specify)"
* Check that every column had the right data type
* Fix blank values

# Some DAX formulas I wrote
Average Salary = AVERAGE(Survey[Salary Number])

Happiness with Salary = AVERAGE(Survey[Q6 - Salary Happiness])

% Career Switchers =
DIVIDE(
    CALCULATE(COUNTROWS(Survey), Survey[Q2 - Career Switch] = "Yes"),
    COUNTROWS(Survey)
)

# What's in the dashboard

* Cards showing total respondents and  average age
* A bar chart comparing average salary by job title
* A chart showing the most popular programming languages
* A breakdown of respondents by country
* Happiness scores for salary and work/life balance
* Salary comparison by gender
* Filters so you can click on a job title, country, or gender and see the dashboard change

# What I learned
Data Scientist is highiest job salary, 
85% of data architect are male and 
Favorite programming language for data analyst is python by 255 of voter 
# See the live dashboard
You don't need to download anything. Click here to view it: [view the live dashboard](https://app.powerbi.com/groups/me/reports/afa9e669-12e4-4b51-b7d7-677cfa889318/f52329e375eceb6b172f?experience=power-bi)

