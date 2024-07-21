# Massachussets Hospital Dashboard Challenge
Maven Analytics provided 4 questions for a high level dashboard to answer. 
- The patients being admitted or readmitted
- Average Length of stay in the hospital
- Average cost of visit  
- Number of procedures covered by insurance

The challenge was you are assumed to have knowledge on hospitals, you need to understand the data given and make your own schema, and decide & discover what KPIs are appropriate in the dashboard.

**This is my ongoing dashboard project from Maven Analytics. Not yet done with the percent changes on KPI but will make the changes**

## Why create this dashboard?
- More than a week ago, I saw a couple of people on linkedin post their dashboard on Maven Analytics Hospital Challenge and I noticed that they're presenting KPI for average length of stay in hospital without regard to type of encounter (is it admission, visit, or readmission?). I disagree to this because I thought a hospital visit is shorter than admission (admission surely take more hours than visit). So my vision is present average length of stay by category.
- I though this was an opportunity to apply custom date slicer and challenge myself to write more measures than create calculated columns. 

## What is this dashboard?
This dashboard is a high level dashboard about the operations and finance of Massachussets General Hospital. The questions given by maven analytics mainly focuses on operations and finance so I figured I'd create dashboard for each.

**Aside from the calendar table (a calculated table), I've tried to avoid doing more calculated tables because I wanted to try a bit of complex dax. From this dashboard, I've learned that custom date slicer is hard especially if you have overlapping date options and doing complex dax will only slow down the report**

### Operations Dashboard
Metrics within the rounded boxes answer these questions: 
- The patients being admitted or readmitted
- Average Length of stay in the hospital

For this dashboard, end users will be able to get a glimpse overall performance of the hospital through North Start KPIs presented on the left side of the dashboard, and number of patients, their length of stay, and the reasons of their admission/readmission/visit. 


![12](https://github.com/user-attachments/assets/5d049aec-9eda-4848-9194-72f3bbefab68)

### Finance Dashboard
Metrics within the rounded boxes answer these questions: 
- Average cost of visit  
- Number of procedures covered by insurance

This Finance Dashboard will help end users not only answer their questions about the cost of visit and the number of procedures performed but also observe gross revenue and its composition to type of encounter and different payers.

![11](https://github.com/user-attachments/assets/f5c70c53-0640-457d-95d6-818767bac073)
