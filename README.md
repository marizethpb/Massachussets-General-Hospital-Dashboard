# Massachussets Hospital Dashboard Challenge
Maven Analytics provided 4 questions for a high level dashboard to answer. 
- The patients being admitted or readmitted
- Average Length of stay in the hospital
- Average cost of visit  
- Number of procedures covered by insurance

The challenge was you are assumed to have knowledge on hospitals, you need to understand the data given and make your own schema, and decide & discover what KPIs are appropriate in the dashboard.

**This is my ongoing dashboard project from Maven Analytics. Not yet done with the percent changes on KPI but will push changes**

## Why create this dashboard?
- More than a week ago, I saw a couple of people on linkedin post their dashboard on Maven Analytics Hospital Challenge and I noticed that they're presenting KPI for average length of stay in hospital without regard to type of encounter (is it admission, visit, or readmission?). I disagree to this because I thought a hospital visit is shorter than admission (admission surely take more hours than visit). So my vision is present average length of stay by category.
- I though this was an opportunity to apply custom date slicer and challenge myself to write more measures than create calculated columns. 

## What is this dashboard?
This dashboard is a high level dashboard about the operations and Finance of Massachussets General Hospital. The questions given by maven analytics mainly focuses on operations and finance so I figured I'd create dashboard for each.

**Aside from the calendar table (a calculated table), I've tried to avoid doing more calculated tables because I wanted to try a bit of complex dax. From this dashboard, I've learned that custom date slicer is hard specially if you have overlapping date options and doing complex dax will only slow down the report**

### Operations Dashboard
Metrics within the rounded boxes answer these questions: 
- The patients being admitted or readmitted
- Average Length of stay in the hospital

For this dashboard, end users will be able to get a glimpse overall performance of the hospital through North Start KPIs presented on the left side of the dashboard, and number of patients, their length of stay, and the reasons of their admission/readmission/visit. 

![image](https://github.com/user-attachments/assets/75a1daff-a877-4bc5-9d50-3ef63a6cfa79)

### Finance Dashboard
Metrics within the rounded boxes answer these questions: 
- Average cost of visit  
- Number of procedures covered by insurance

This Finance Dashboard will help end users not only answer their questions about the cost of visit and the number of procedures performed but also the gross revenue and its composition to type of encounter and different payers.

![image](https://github.com/user-attachments/assets/b617742a-fc45-4c1f-a194-856765fbc0e5)

