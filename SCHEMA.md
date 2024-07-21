# Data Model
![image](https://github.com/user-attachments/assets/49df3e90-b72b-4d81-a4c0-bf38bd429bee)

Shown above is the data model for the dashboard which includes the payers, encounters, procedures, period, calendar, patients, ops measures, and finance measures table. Its a mini snowflake schema with procedures as the fact table and encounter & calendar as inner dimension tables. Notice the circular-like relationship between calendar, encounter, and procedures table. For that, I deactivated the relationship between calendar and procedures and set the procedures and encounter table relationship as the default. I'd just use userelationship function to filter procedures table with calendar table.

## Measures Table
![image](https://github.com/user-attachments/assets/76749267-20f2-47a9-a675-f513821ee473)
The standalone tables on the top left are the measures table for each of Operations and Finance Dashboard.

## Given Tables
![image](https://github.com/user-attachments/assets/0e743ec4-60b2-4cc2-8e83-26b14173a2e3)

The tables given by Maven Analytics are the
- Payers Table. Which consists of entities that paid for claim costs.
- Encounters Table. Which consists of hospital encounters from 2011 to 2022.
- Procedures Table. Which consists of procedures performed to each encounter from 2011 to 2022.
- Patients Table. Which consists of patients id and their deathdate.

Originally, the tables have more columns than what is presented in the data model. I removed those columns because I find it unnecessary for my vision of the dashboard

## Tables I added
![image](https://github.com/user-attachments/assets/7ec59711-a15b-4ad7-8a21-6649e8372bdb)

- Calendar Table. I created a date table for faster querying and to bridge the encounter and procedures table.
- Periods Table. I created custom date slicer do I need another table for filtering the calendar table aside from needing a reference column for slicer dropdown. 
