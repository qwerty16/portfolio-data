# Helpdesk Dashboard

https://public.tableau.com/views/HelpDeskDashboard_16514411469530/Helpdesk?:language=en-GB&publish=yes&:display_count=n&:origin=viz_share_link

Dashboard of information about the performance of a helpdesk including areas recommended for improvement.
First I wrangled the data in excel and then created the dashboard in Tableau.
Dataset is from Data.world’s “real world fake data” project of fictional helpdesk tickets: https://data.world/markbradbourne/rwfd-real-world-fake-data/workspace/file?filename=Help+Desk.csv

## Design Choices
1.	Using only a few colours and one highlight colour for areas that may need attention –using colour as a pre-attentive attribute so that the viewers eye jumps immediately to the important areas, saving time and effort for my busy persona 
2.	Making the viz as simple as possible by adding labels and tooltips and removing axes to remove visual clutter and make the charts easy to understand
3.	Having text information (axis labels etc) be horizontal to make them quick and easy to read

## How my plan changed and what I learned during the process
I originally planned this to be a single page viz but found that if I added all the vizes to one screen they ended up small, cluttered and difficult to understand. I also felt that it was easier to control the flow of the user throughout the viz story by using story points.
I created my persona and KPIs before fully exploring all of the data and was surprised when almost none of the tickets were resolved in less than 15 days, but this then added useful points to the story which clearly shows the usefulness of vizes in highlighting information that is difficult to glean from tabular data.
I had to create and used multiple measures, parameters and aliases throughout the project which I had not done before. I also made a chart with a dual axis and syncronised the axes. I learned how to format numbers in a variety of ways according to the best way to communicate information to the viewer.
I found having an original project proposal written before starting really helpful to guide me towards my end goal and I referred back to it several times throughout the project when I was uncertain of what direction to go in next.


## Original Proposal
### Executive Summary
IT support helpdesks need to be able to show that they are resolving tickets quickly (usually more severe tickets need to be resolved more quickly) and to their customer’s satisfaction.
A manager of a helpdesk would also need to keep an eye on how many tickets are currently open to establish how much work the team currently has.
Information about the categories of tickets being created helps to identify potential major issues quickly. 
I would like to be able to try to learn to use Tableau to quickly and clearly communicate key metrics.
### Why
Goals:
•	To quickly understand the help desk performance against KPIs, and how this differs from the previous month
•	To have a view of how the KPIs have changed over the last month, quarter or year (user selectable)
•	To be able to identify trends in the tickets created today and how these are different to the previous day
### Who
Audience
Subject matter expert help desk manager Barry understands what tickets are but needs to know if team goals are being met
Persona
•	Name: Barry
•	Age: 35
•	Gender: Male
Goals  
•	Comparisons of monthly KPIs compared to the previous month, quarter or year
•	Total number of tickets open compared to the previous day
•	Severity vs days open 50% target on each
o	High priority tickets resolved within 3 days
o	Medium priority tickets resolved within 5 days
o	Low priority tickets resolved within 10 days
o	Unassigned priority tickets resolved within 20 days
•	Satisfaction score
o	80% satisfied or highly satisfied
o	50% highly satisfied
•	Tickets opened today by issue category and department with absolute change compared to the previous day to identify potential issues
Challenges and needs
•	Mostly interested in KPIs that might be close to failing, those that have clearly passed or failed need less attention
•	Not interested in individual tickets or users, just needs overall trends
Context
•	Visits dashboard daily on desktop PC
•	Visits several times a day to see live information about KPIs with less detailed information about previous performance and focus on current months’ data
### What
Data
Data.world’s “real world fake data” project contains a help desk dataset of fictional helpdesk tickets: https://data.world/markbradbourne/rwfd-real-world-fake-data/workspace/file?filename=Help+Desk.csv
Data Quality
Data does not have incorrectly values, dates or labels
We will not be using the ticket number, user’s first/last name or ticket type columns, these can be hidden from the model.
Data Timeliness
8 months of ticket data from March to October 2020
### How
Single page dashboard with an alternative mobile layout containing fewer graphs
Global slicer to adjust the date range of all charts
KPI dial for KPIs with a red section for missing target, a marker for the current day and a marker for the previous month
Line charts of KPIs over the selected timeframe to show changes over time
Info on each KPI to make it clear what the goal is and what is being measured
Clustered horizontal bar charts of the current day vs previous day issue and department
Challenges
Reshaping data to get a snapshot of the state of the help desk at different points in time
