---
layout: post
title: "Building an analytics feature that answer business questions"
excerpt: "An example of making sophisticated statistical analysis accessible through productisation."
categories: [analytics products]
share: true
image:
  feature:
  credit:
  creditlink:
---


Survival analysis is an statistical method usually used in the medical field as it's useful in analysing the expected duration of time until an event happen. In HR analtyics, reporting on and predicting (thereby preventing) employee churn (employee turn-over) is one of the important topics. With a data science and engineering team, I've built Survival Curves feature into the [OrgVue](https://orgvue.com) that doesn't require data processing or writing codes to get an output.
This feature now helps many organisations to better understand when and where employee attrition is happening and plan and execute on retention programmes.

#### Process

**1. Defined objectives and key business questions**

* To prevent top talent from leaving the organisation,
* Understand attrition pattern for a particular time period – when, where and why is happening (Descriptive)
  * **When** employees are likely to leave in their tenure
  * **Where** attrition is occurring (i.e. which segment has higher flight risk)? 
  * How does the trend differ by group or cohort?
  * How does the trend change **over time**?
* **Who** is likely to leave in the next year? (Predictive)
* What can we do to affect turn-over? (Prescriptive) 
  * Identify key attributes causing attrition


**2. Created a list of possible analytics and reporting features can help answer different business questions**
* Survival Analysis: for each group shows the percentage of employees that leave after a given tenure probability
* Cohort Analysis for retention/ turnover rates : employee lifetime by cohort, actual numbers based on historic data
* Attrition drivers / predictors using Decision tree: show top drivers and the degree of influence
* Employees with high flight risk : categorise employees based on risk level (likelihood of leaving), show number of employees with high flight risk by dimension
* Summary report that shows turn-over related KPIs and changes overtime

**3. Prioritsed Survival Analysis and defined minimal requirements for release**

Based on investigation of current technical viability and target users' needs, decided to develop Survival Analysis focusing on the business question: "How the likelihood of staying/ leaving differ by group?"

Minimal functional requirements included:
* Works with the data that contains start and leave dates for each employee
* User can toggle between three curves, i.e. Surival, Turnover (Cummulative) and Turnover (Period). The survival function is calculated in the background
* If the data has addition dimension such as gender, it draws curve for each group

Control Panel mock-ups:<br>
![](https://s3.eu-west-2.amazonaws.com/lubynoel-portfolio/survival-curves-ui-controls-1.png)

![](https://s3.eu-west-2.amazonaws.com/lubynoel-portfolio/survival-curves-ui-controls-2.png)

#### Exmaple product screenshots

The image below shows example Survival, Turnover (Cummulative) and Turnover (Period) curves produced for female and male group.

<style>
* {
    box-sizing: border-box;
}

.column {
    float: left;
    width: 50%;
    padding: 5px;
}

/* Clearfix (clear floats) */
.row::after {
    content: "";
    clear: both;
    display: table;
}

/* Responsive layout - makes the three columns stack on top of each other instead of next to each other */
@media screen and (max-width: 500px) {
    .column {
        width: 100%;
    }
}
</style>

<div class="row">
  <div class="column">
      <img src="https://s3.eu-west-2.amazonaws.com/lubynoel-portfolio/survival-curves-1-survival-prop.png">
  </div>
<div class="row">
  <div class="column">
     <img src="https://s3.eu-west-2.amazonaws.com/lubynoel-portfolio/survival-curves-2-turnover-prop.png">
  </div>
<div class="row">
  <div class="column">
     <img src="https://s3.eu-west-2.amazonaws.com/lubynoel-portfolio/survival-curves-3-trunover-rate.png">
  </div>
</div>
