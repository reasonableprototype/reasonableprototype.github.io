---
layout: post
title: "Making analytics accessible"
excerpt: "Getting Survival Curves on user's finger"
categories: [analytics products]
share: true
image:
  feature:
  credit:
  creditlink:
---

Survival Curves is one of the features provided for Attrition and Retention Analysis as part of Advanced Org Analytics Module in [OrgVue](https://orgvue.com).


#### Objectives and business questions

* To prevent top talent from leaving the organisation,
* Understand attrition for a particular time period – when, where and why is happening (Descriptive)
  * **When** employees are likely to leave (tenure/ lifetime)
  * **Where** attrition is occurring? 
  * Other related metrics (turnover rate) by group/ cohort
  * How does the trend change **over time**?
* **Who** is likely to leave in the next year? (Predictive)
* What can we do to affect turnover? (Prescriptive) 
  * Identify key attributes causing attrition

#### Actions enabled
* Focus attention the most at-risk employees / segments
* Determine the most effective retention strategies and create programmes

#### A series of analytics and reporting features can help answer different business questions
* Survival Analysis: for each group shows the percentage of employees that leave after a given tenure (can be calculated from hazard rate) probability
* Cohort Analysis for actual retention/ turnover rates : Employee lifetime by cohort, actual numbers based on historic data
* Attrition drivers / predictors using Decision tree: Show what are the key factors contributing to attrition , show top drivers and the degree of influence
* Employees with high flight risk : Categorise employees based on risk level (likelihood of leaving), show number of employees with high flight risk by dimension
* Other related KPIs and changes overtime

#### MVP

Q1: How the likelihood of staying/ leaving differ by group?

Features:
Using start and end date produces 2 charts - Line graph for hazard distribution curve (turnover), Stepped line graph for survival curve using employee start and end date data
Option to display confidence interval
Use Color Panel to choose group – dependant on data availability
Number of groups can be ranged from 2 to 30+ e.g. country offices
Ability to set a control group
An toggle to split and plot all groups on one chart

![](https://s3.eu-west-2.amazonaws.com/lubynoel-portfolio/survival-curves-ui-controls-1.png)

![](https://s3.eu-west-2.amazonaws.com/lubynoel-portfolio/survival-curves-ui-controls-2.png)


![](https://s3.eu-west-2.amazonaws.com/lubynoel-portfolio/3-curves.png)
