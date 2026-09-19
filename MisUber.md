Yes — I get exactly what you mean. You want a Pareto/80-20 preparation sheet: not 100 topics, but the smallest set of high-impact topics/questions that are most likely to matter for this MIS Executive role.

I’m basing this primarily on the actual JD screenshots you provided, especially the repeated responsibilities and the listed critical skills, rather than giving you a generic MIS syllabus.

One important point: nobody can guarantee the exact assessment questions, but we can aggressively prioritize the areas that the JD itself emphasizes.

Below is ready-to-paste .md content for your GitHub study file.

# MIS Executive – Uber Technologies
## 80/20 Pareto Preparation Guide
### Assessment + Interview | Hyderabad

> Goal: Prepare the smallest number of high-impact topics that are most likely to cover the majority of the assessment/interview requirements.

---

# 1. ROLE AT A GLANCE

## Target Role

**MIS Executive – Uber Technologies, Hyderabad**

## Core purpose of the role

This role appears to combine:

- MIS reporting
- Excel/data analysis
- Performance dashboards
- Operational metrics
- Scheduling/workforce management
- Data and insights
- Process improvement
- Billing & invoicing
- Inventory management
- Stakeholder communication
- Issue identification and resolution

The JD specifically mentions:

- Google Sheets
- MS Excel / MS Office
- Advanced Excel
- IEX
- Power BI
- Tableau
- Data Studio
- Scheduling
- Performance dashboards
- Reporting accuracy
- Performance monitoring
- Analytical/problem-solving ability
- Presentation skills

---

# 2. THE 80/20 PRIORITY MAP

## 🔴 PRIORITY 1 — MUST KNOW

These are the topics I should spend most of my preparation time on.

### 1. Advanced Excel
### 2. MIS Reporting
### 3. KPI / Performance Metrics
### 4. Pivot Tables
### 5. VLOOKUP / XLOOKUP
### 6. SUMIFS / COUNTIFS / IF / IFERROR
### 7. Data Cleaning & Validation
### 8. Dashboard Fundamentals
### 9. Data Interpretation & Problem Solving
### 10. SLA / TAT / Productivity / Quality
### 11. Scheduling / Workforce Management Basics
### 12. Stakeholder & Report Communication

---

# 3. PRIORITY 2 — SHOULD KNOW

These can differentiate me in the interview.

- Power BI basics
- Power Query basics
- Tableau basics
- Google Data Studio / Looker Studio basics
- IEX basics
- Forecasting
- Staffing
- Adherence
- Utilization
- Shrinkage
- Billing & invoicing
- Reconciliation
- Inventory management
- Variance analysis
- Trend analysis

---

# 4. PRIORITY 3 — LOW PRIORITY

Do NOT spend excessive time here before the assessment.

- Advanced DAX
- Complex Power BI architecture
- Advanced Tableau
- Advanced VBA
- Complex SQL
- Advanced statistics
- Advanced Python
- Advanced forecasting models

These are not the main emphasis visible in the JD.

---

# 5. TOP 10 THINGS I MUST BE ABLE TO DO

If I have very limited preparation time, I should be able to do these 10 things confidently:

1. Create a Pivot Table.
2. Use VLOOKUP/XLOOKUP.
3. Use SUMIFS and COUNTIFS.
4. Use IF and IFERROR.
5. Calculate productivity, quality, SLA and TAT.
6. Clean a messy Excel dataset.
7. Identify trends and performance gaps.
8. Build a simple operational dashboard.
9. Explain what MIS is and what an MIS Executive does.
10. Analyze a performance problem and explain the likely causes using data.

---

# 6. EXCEL — HIGHEST PRIORITY

## A. Formulas I MUST KNOW

### Basic

```excel
=SUM(A1:A10)
=AVERAGE(A1:A10)
=COUNT(A1:A10)
=COUNTA(A1:A10)
=MAX(A1:A10)
=MIN(A1:A10)

Conditional

=IF(A2>=90,"Met","Below Target")

Error handling

=IFERROR(A2/B2,0)

Conditional counting

=COUNTIF(B:B,"Team A")

=COUNTIFS(B:B,"Team A",C:C,"Completed")

Conditional sum

=SUMIF(B:B,"Team A",D:D)

=SUMIFS(D:D,B:B,"Team A",C:C,"Completed")


---

7. VLOOKUP / XLOOKUP

VLOOKUP

Basic syntax:

=VLOOKUP(lookup_value,table_array,column_number,FALSE)

Example:

=VLOOKUP(A2,Sheet2!A:D,4,FALSE)

XLOOKUP

Basic syntax:

=XLOOKUP(lookup_value,lookup_array,return_array)

Example:

=XLOOKUP(A2,Sheet2!A:A,Sheet2!D:D)

Interview Question

Q: Difference between VLOOKUP and XLOOKUP?

Answer:

> XLOOKUP is a more flexible lookup function. It allows separate lookup and return ranges and can return values from either side of the lookup column. VLOOKUP traditionally searches from left to right and uses a column index number.




---

8. PIVOT TABLES — VERY IMPORTANT

What is a Pivot Table?

A Pivot Table summarizes large datasets quickly.

Example:

Raw data:

Agent	Team	Volume	Quality

A	Team 1	100	95%
B	Team 1	120	97%
C	Team 2	80	90%
D	Team 2	110	96%


Question:

> What is the total volume by team?



Pivot:

Team	Total Volume

Team 1	220
Team 2	190


I should know:

Rows

Columns

Values

Filters

Sum

Count

Average

Grouping

Sorting

Filtering



---

9. DATA CLEANING

I should know how to check for:

Duplicate records

Blank cells

Incorrect dates

Numbers stored as text

Inconsistent names

Extra spaces

Incorrect formats

Missing values

Invalid values


Important Excel tools:

Remove Duplicates

Filter

Sort

Conditional Formatting

Data Validation

Text to Columns

TRIM

Find & Replace



---

10. MIS — WHAT I MUST UNDERSTAND

What is MIS?

MIS = Management Information System.

In an operations environment, MIS generally involves:

Collect Data
     ↓
Clean Data
     ↓
Analyze Data
     ↓
Calculate KPIs
     ↓
Create Reports
     ↓
Create Dashboards
     ↓
Provide Insights
     ↓
Support Business Decisions

Interview Answer

> MIS involves collecting, validating, analyzing and presenting operational data through reports and dashboards so that management can monitor performance and make informed decisions.




---

11. KPI

KPI = Key Performance Indicator.

A KPI measures performance against a defined business objective or target.

Examples:

Productivity

Quality

SLA

TAT

Attendance

Adherence

Utilization

Volume

Error rate



---

12. PRODUCTIVITY

Basic concept:

Productivity = Output / Input

Example:

An employee processes 120 cases in 8 hours.

120 / 8 = 15 cases per hour

Interview Question

> How would you measure employee productivity?



Answer

> I would define the appropriate output for the process, divide it by the relevant input such as productive hours, and compare the result against the established target or historical baseline.




---

13. QUALITY / ACCURACY

Basic formula:

Accuracy % = Correct Transactions / Total Transactions × 100

Example:

98 correct out of 100:

98 / 100 × 100 = 98%


---

14. SLA

SLA = Service Level Agreement.

It defines an expected service standard.

Example:

> A report must be delivered before 10:00 AM every working day.



If the report is delivered after the agreed deadline, the SLA may be missed.


---

15. TAT

TAT = Turnaround Time.

It measures the time taken to complete a task.

Example:

Request received:

10:00 AM

Report delivered:

12:00 PM

TAT:

2 hours


---

16. SLA vs TAT

SLA

The agreed service standard/deadline.

TAT

The actual time taken to complete the task.

Simple way to remember:

SLA = What standard was promised?
TAT = How long did it actually take?


---

17. VARIANCE ANALYSIS

Variance means the difference between expected/target and actual performance.

Example:

Target productivity:

15 cases/hour

Actual:

12 cases/hour

Variance:

12 - 15 = -3 cases/hour

The next question is:

> WHY is there a variance?



Possible causes:

Volume changes

Staffing shortage

Absenteeism

System issues

Process changes

Training

Schedule adherence

Data/reporting issue

Workflow problems



---

18. DASHBOARD — VERY IMPORTANT

A good dashboard should allow management to answer:

1. What is happening?


2. Where is the problem?


3. How large is the problem?


4. When did it start?


5. Which team/agent/process is affected?


6. What action is required?



Example Operations Dashboard

KPI Cards

Total Volume
Completed Volume
Pending Volume
Productivity
Quality
SLA
Attendance
Adherence

Charts

Volume by date

Productivity by team

Quality by team

SLA trend

Pending volume

Performance comparison



---

19. POWER BI — BASIC LEVEL

I should know these terms:

Power Query

Data Cleaning

Data Model

Relationships

Measures

Calculated Columns

DAX

Filters

Slicers

Visualizations

Dashboard

Report

Data Refresh


Interview Question

Q: Excel vs Power BI?

Answer:

> Excel is highly useful for spreadsheet-based analysis, calculations and operational reporting. Power BI is designed more specifically for interactive dashboards, data modeling, visualization and reporting across multiple data sources.




---

20. POWER QUERY

Basic understanding:

Power Query is used for:

Importing data

Cleaning data

Transforming data

Combining data

Preparing data for analysis


Remember:

Raw Data
   ↓
Power Query
   ↓
Clean/Transform
   ↓
Power BI / Excel


---

21. TABLEAU / DATA STUDIO

I don't need advanced knowledge initially.

I should understand that they are business intelligence/data visualization tools used to:

Connect to data

Analyze data

Create visualizations

Build dashboards

Monitor KPIs

Share insights



---

22. IEX / WORKFORCE MANAGEMENT

The JD specifically mentions IEX.

I should understand these concepts:

Forecasting
     ↓
Required Staffing
     ↓
Scheduling
     ↓
Actual Operations
     ↓
Adherence Monitoring
     ↓
Intraday Management

Forecasting

Estimate future workload/volume.

Staffing

Determine how many people are needed.

Scheduling

Assign employees to appropriate shifts/time periods.

Adherence

Compare actual activity against the scheduled activity.


---

23. SCHEDULING

The JD specifically asks for knowledge of scheduling basics.

I should understand:

Shift planning

Staffing requirements

Workload

Employee availability

Break schedules

Coverage

Absenteeism

Peak periods

Shrinkage

Adherence


Possible question:

> What would you consider when creating an employee schedule?



Answer:

> I would consider forecasted workload, required staffing, employee availability, shift requirements, breaks, planned leave, coverage requirements and operational constraints.




---

24. BILLING & INVOICING

Basic logic:

Volume
×
Rate
=
Billing Amount

Example:

10,000 transactions × ₹2
= ₹20,000

But before finalizing billing:

Operational Data
       ↓
Validate Volume
       ↓
Check Rate
       ↓
Reconcile
       ↓
Identify Variance
       ↓
Finalize Billing


---

25. RECONCILIATION

Reconciliation means comparing two sources to ensure they agree.

Example:

Operational report:

10,000 transactions

Billing report:

10,500 transactions

Difference:

500

I should investigate:

Duplicate records

Missing records

Different reporting periods

Incorrect classifications

Data extraction problems

Rate/volume mismatch



---

26. INVENTORY MANAGEMENT

Basic formula:

Opening Inventory
+
Received
-
Consumed
=
Expected Closing Inventory

Example:

Opening = 1,000
Received = 500
Consumed = 300

Expected Closing = 1,200

If actual closing = 1,150:

Variance = 50

The important skill is identifying and investigating the variance.


---

27. THE MOST IMPORTANT PROBLEM-SOLVING FRAMEWORK

For almost every scenario question, use:

1. Validate
2. Identify
3. Analyze
4. Find Root Cause
5. Communicate
6. Take Corrective Action
7. Monitor

Example:

> Productivity dropped by 15%.



Answer structure:

1. Validate

Check whether the data/report is correct.

2. Identify

Find which team, agent, shift or period is affected.

3. Analyze

Compare with historical performance.

4. Root Cause

Check:

Volume

Staffing

Absenteeism

System issues

Process changes

Adherence

Training


5. Communicate

Share the finding with the relevant stakeholder.

6. Correct

Implement or coordinate the required action.

7. Monitor

Check whether performance improves.


---

28. TOP 25 QUESTIONS I SHOULD PREPARE

Excel

1. What is VLOOKUP?

2. What is XLOOKUP?

3. Difference between VLOOKUP and XLOOKUP?

4. What is a Pivot Table?

5. What is SUMIFS?

6. What is COUNTIFS?

7. What is IFERROR?

8. How do you remove duplicates?

9. How do you identify missing data?

10. How do you create a dashboard in Excel?


---

MIS

11. What is MIS?

12. What is KPI?

13. What is SLA?

14. What is TAT?

15. What is productivity?

16. What is variance?

17. What is reconciliation?

18. How do you ensure report accuracy?

19. How would you investigate a performance decline?

20. What should an operational dashboard contain?


---

Workforce / Operations

21. What is forecasting?

22. What is scheduling?

23. What is adherence?

24. What is IEX?

25. How would you handle an unexpected increase in workload?


---

29. TOP INTERVIEW QUESTIONS FOR MY PROFILE

Because my current experience is Trust & Safety, I should prepare these particularly well.

Q1. Tell me about yourself.

Key structure:

BCA
↓
Current Wipro Trust & Safety role
↓
High-volume operations
↓
Quality + productivity + accuracy
↓
Trend analysis/process improvement
↓
Interest in data-driven operations
↓
Transition to MIS


---

30. Q2. Why do you want to move from Trust & Safety to MIS?

Suggested answer:

> My current role has given me strong exposure to operational metrics, quality, productivity, compliance and trend analysis. Over time I became particularly interested in the analytical side of operations—understanding performance, identifying patterns and improving processes. I want to move into MIS because it allows me to apply these skills more directly through reporting, dashboards and data analysis.




---

31. Q3. You don't have direct MIS experience. Why should we hire you?

Suggested answer:

> Although my current designation is in Trust & Safety, many of my responsibilities are transferable to MIS operations. I work in a high-volume environment where accuracy, quality, productivity and compliance are critical. I've also worked with trend analysis and process improvement. My BCA background gives me a technical foundation, and I am building hands-on skills in advanced Excel, reporting and dashboards. I believe I can bring strong operational discipline while quickly learning the specific MIS processes and tools.




---

32. Q4. How does your current role relate to MIS?

Strong connection:

Current Trust & Safety
        ↓
Operational Data
        ↓
Quality Metrics
        ↓
Productivity Metrics
        ↓
Compliance
        ↓
Trend Analysis
        ↓
Process Improvement
        ↓
MIS

My experience already involves:

High-volume operations

Accuracy

Quality

Productivity

Compliance

Trend analysis

Process improvement

Issue identification


My resume documents these areas in my current Wipro role.


---

33. Q5. How do you ensure report accuracy?

Answer:

> I would validate the source data first, check for missing or duplicate records, verify formulas and calculations, compare totals against source systems, perform reasonableness checks, and review the final report before sharing it. For recurring reports, I would also maintain a standard validation checklist.




---

34. Q6. What would you do if a stakeholder says your report is incorrect?

Answer:

> I would first understand the specific discrepancy rather than immediately assuming either side is correct. I would verify the source data, definitions, reporting period, formulas and filters. If I find an error, I would correct it and communicate the update. If the report is correct, I would explain the calculation and source data clearly with supporting evidence.




---

35. Q7. What if an urgent report is requested while I am working on another report?

Answer:

> I would first understand the urgency, deadline and business impact of both requests. I would communicate the expected timelines to the stakeholders, prioritize based on business criticality, and ensure that speed does not compromise data accuracy. If necessary, I would ask for prioritization from the relevant manager.




---

36. Q8. What would you do if data from two reports doesn't match?

Answer:

> I would reconcile the two datasets by checking the reporting period, source, filters, definitions, duplicate records, missing records and calculation logic. Once I identify the source of the discrepancy, I would document it and communicate the corrected numbers and reason for the difference.




---

37. Q9. What would you do if productivity suddenly falls?

Answer:

> I would first validate the data, then segment the performance by team, employee, shift and time period. I would compare it with historical trends and investigate possible causes such as volume changes, absenteeism, staffing gaps, system issues, adherence or process changes. After identifying the likely cause, I would communicate the finding and monitor the corrective action.




---

38. Q10. What makes a good MIS report?

Answer:

A good MIS report should be:

Accurate

Timely

Relevant

Easy to understand

Consistent

Actionable

Properly validated


The report should help management answer:

> What happened?



> Why did it happen?



> Where is the problem?



> What action is required?




---

39. MY 80/20 STUDY ORDER

If I have only 2 days:

🔴 Day 1 — Highest Priority

1. Excel formulas

IF
IFERROR
SUMIF
SUMIFS
COUNTIF
COUNTIFS
VLOOKUP
XLOOKUP

2. Pivot Tables

3. Data Cleaning

4. KPI calculations

Productivity
Quality
SLA
TAT
Variance

5. MIS fundamentals


---

40. DAY 2

Morning

Excel Practical

Build one complete report using:

Raw data

Cleaning

Formulas

Pivot Table

Charts

KPIs



---

Afternoon

Workforce concepts

Learn:

Forecasting

Staffing

Scheduling

Adherence

IEX

Utilization

Shrinkage



---

Evening

Interview

Practice:

Tell me about yourself

Why MIS?

Why leave Trust & Safety?

Why should we hire you?

No direct MIS experience?

Productivity decline scenario

Data mismatch scenario

Urgent report scenario

Difficult stakeholder scenario



---

41. THE 20% I SHOULD MEMORIZE

If I forget everything else, remember these:

MIS
= Data → Analysis → Reporting → Insights

KPI
= Measure of performance

SLA
= Agreed service standard

TAT
= Time taken to complete a task

Productivity
= Output / Input

Quality
= Correct / Total × 100

Variance
= Actual - Target

Reconciliation
= Compare two sources and investigate differences

Pivot Table
= Quickly summarize data

VLOOKUP/XLOOKUP
= Find information from another dataset

SUMIFS/COUNTIFS
= Conditional aggregation

Dashboard
= Visual representation of important KPIs

Forecasting
= Estimate future workload

Staffing
= Determine required people

Scheduling
= Assign people/time to meet workload

Adherence
= Actual activity vs scheduled activity

Root Cause Analysis
= Find why the problem happened


---

42. MY BIGGEST INTERVIEW ADVANTAGE

I should not try to convince the interviewer that I already have years of MIS experience.

Instead, position myself as:

> Operations professional + analytical mindset + BCA background + strong accuracy/quality discipline + rapidly developing MIS/Excel skills.



My current experience includes high-volume content review, quality/compliance, productivity, trend analysis and process improvement. These are transferable to operational MIS work.


---

43. MY BIGGEST GAP

The biggest gap is:

Direct MIS Tool Experience

Especially:

Advanced Excel

IEX

Power BI

Tableau

Data Studio


Therefore, I should NOT falsely claim production experience.

If asked:

> "Have you used IEX?"



Answer honestly:

> "I haven't used IEX extensively in a production environment yet, but I understand the basic workforce-management concepts around forecasting, scheduling and adherence, and I'm actively building my knowledge."




---

44. WHAT NOT TO WASTE TIME ON

Do NOT spend most of my remaining preparation time learning:

Advanced Python
Advanced SQL
Advanced DAX
Advanced VBA
Advanced Tableau
Advanced Statistics
Machine Learning

Unless the assessment specifically introduces them.

The JD emphasis is much more strongly aligned with:

Excel
MIS
Reporting
Dashboards
Operations
Scheduling
IEX
Performance Metrics
Problem Solving
Communication


---

45. FINAL 80/20 CHECKLIST

Before entering the assessment, I should be able to answer YES to all of these:

[ ] I can use IF.

[ ] I can use IFERROR.

[ ] I can use SUMIFS.

[ ] I can use COUNTIFS.

[ ] I can use VLOOKUP.

[ ] I can use XLOOKUP.

[ ] I can create a Pivot Table.

[ ] I can clean a dataset.

[ ] I can calculate productivity.

[ ] I can calculate quality.

[ ] I understand SLA.

[ ] I understand TAT.

[ ] I understand variance.

[ ] I understand reconciliation.

[ ] I understand KPI.

[ ] I can explain MIS.

[ ] I can create a basic dashboard.

[ ] I understand Power BI basics.

[ ] I understand IEX at a conceptual level.

[ ] I understand forecasting.

[ ] I understand scheduling.

[ ] I understand adherence.

[ ] I can explain how my Trust & Safety experience transfers to MIS.

[ ] I can explain why I want MIS.

[ ] I can solve a performance problem using data.



---

46. THE ONE FORMULA FOR THE WHOLE INTERVIEW

When given any operational problem:

DATA
 ↓
VALIDATE
 ↓
COMPARE
 ↓
IDENTIFY GAP
 ↓
SEGMENT
 ↓
FIND ROOT CAUSE
 ↓
COMMUNICATE
 ↓
ACTION
 ↓
MONITOR

If I can demonstrate this thinking consistently, I can handle many MIS scenario questions even when the exact question is unfamiliar.


---

47. FINAL PRIORITY

🔥 MUST MASTER

1. Advanced Excel basics


2. VLOOKUP/XLOOKUP


3. SUMIFS/COUNTIFS


4. Pivot Tables


5. Data Cleaning


6. KPI calculations


7. MIS reporting


8. SLA/TAT/Productivity/Quality


9. Dashboard fundamentals


10. Data interpretation


11. Problem-solving/root-cause analysis


12. Scheduling/WFM basics



⚡ KNOW CONCEPTUALLY

13. IEX


14. Power BI


15. Power Query


16. Tableau


17. Data Studio


18. Forecasting


19. Staffing


20. Adherence


21. Billing/Reconciliation


22. Inventory/Variance



💤 LOW PRIORITY

23. Advanced DAX


24. Advanced Tableau


25. VBA


26. Advanced SQL


27. Advanced statistics


28. Python




---

48. MY PREPARATION PRINCIPLE

> Don't try to know everything. Become extremely comfortable with the small set of skills that the role repeatedly depends on.



The highest-value combination for this role is:

EXCEL
+
MIS
+
KPI ANALYSIS
+
DASHBOARDS
+
OPERATIONS
+
PROBLEM SOLVING
+
COMMUNICATION

That is my 80/20 preparation target.

### One correction to your expectation

I **wouldn't treat any particular question as "sure-shot"** because we don't have the actual assessment paper. What we *can* do is prioritize what the JD repeatedly emphasizes. The strongest signals in the screenshots are **Excel/MIS reporting, performance dashboards, scheduling/IEX, operational metrics, accuracy/timeliness, analytical problem solving, and communication**.

Your resume gives you a useful foundation for the operational side: high-volume work, accuracy, productivity/quality targets, trend analysis and process improvement are already documented. 0

**My recommendation for the next step:** don't jump straight into the 45-question mock yet. First, take the above `.md` as your **master syllabus**, and then I can build you a **Day-1 practical Excel training pack** with a fake Uber-style MIS dataset, formulas, Pivot Table exercises, KPI calculations, and answers. That will convert this 80/20 list from theory into actual assessment ability.