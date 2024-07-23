# SLA-ticket-Data-Analysis-

Overview of the Dataset
The provided dataset contains two sheets: "Ticket and Date Created" and "Help Desk Ticket". For analysis
purposes, the "Help Desk Ticket" sheet is used, which contains 549 rows and 26 columns. Below are a few
column names and the details they capture about help desk tickets, providing various aspects of ticket
management.
• Ticket ID: Unique identifier for each ticket.
• Team Assigned: The team responsible for handling the ticket.
• Priority: The priority level of the ticket (Emergency, High, Normal, Low).
• Type: The type of ticket (Incident, Problem, Request).
• Status: The current status of the ticket (Open, Closed, Resolved).
• Source: The origin of the ticket (Email, Web, Phone, Other).
• Creation Date: The date the ticket was created.
• Last Updated Date: The most recent date the ticket was updated.
• SLA Due Date: Calculated due date based on SLA criteria.
• Breached SLA?: Calculated Indicator if the ticket breached the SLA.
Objective
The primary objective of this analysis is to enhance the efficiency and effectiveness of help desk operations
by leveraging data-driven insights. This involves a comprehensive examination of the help desk ticket data
to identify patterns, trends, and areas for improvement in support processes. By cleaning and preparing the
dataset, I ensure that the information used is accurate and reliable, forming a solid foundation for subsequent
analysis and providing recommendations to answer the question: Why are SLAs being breached?
A key focus of the analysis is to assess the distribution of workload among different teams and agents. The
analysis aims to provide actionable recommendations to optimize support processes, improve SLA
compliance, and balance workload distribution. This will help in identifying imbalances that may lead to
inefficiencies or employee burnout, ultimately driving improvements in help desk performance, service
quality.
Data Cleaning
1. Removed all duplicate entries.
2. Corrected any incorrect data.
3. Filtered out irrelevant data.
Analysis Performed
1. Total Tickets per Team: Used COUNTIF to tally the total tickets assigned to each team.
2. Total Tickets per Priority: Used COUNTIF to calculate the total tickets per priority level.
3. Total Tickets per Type: Applied COUNTIF to determine the total tickets for each type.
4. Total Open Tickets: COUNTIF was used to count the total open tickets.
5. Total Resolved Tickets: VLOOKUP was used to count the total resolved tickets.
6. Total Closed Tickets: was used to count the total closed tickets.
7. Total Open/Answered Tickets: COUNTIF was used to count the open/answered tickets.
8. Tickets from Each Source: COUNTIF was used to count the tickets from email, web, and phone
sources.
SLA Computation
For SLA computation below following task has been done and to perform below task Advanced excel
function is used :
1. Added a new column "SLA Due Date".
2. Computed SLA for "Incident/Problem" types and indicated "No SLA for Request" for request types.
3. SLA criteria applied:
o Emergency: 4 hours
o High Priority: 3 business days
o Normal: 5 business days
o Low: 10 business days
4. Calculated due dates excluding weekends.
5. Added a column "Breached SLA?" to indicate if the SLA due date was greater than the last updated
date.
Visualization
1. Created a "Summary" worksheet displaying key metrics.
2. Created pivot tables and charts for easier data visualization and analysis.
3.Added slicers for interactive data filtering based on priority, source, type, department, and breached
SLA.
Findings and Recommendations:
Workload Distribution: Uneven workload distribution with certain teams and agents handling
more tickets, leading to SLA breaches.
Performance Analysis: Identified agents with high ticket volumes and SLA breaches.
Establish specialized teams for high-priority tickets.
Recommendations:
Balance ticket distribution.
Allocate additional resources to overburdened agents.
Provide regular training.
Establish specialized teams for high-priority tickets.
