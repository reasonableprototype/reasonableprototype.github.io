---
layout: post
title: "From hypothesis to product enhancements"
excerpt: ""
categories: [analytics products]
share: true
image:
  feature:
  credit:
  creditlink:
---

#### Background

[OrgVue](https://www.orgvue.com/) has a number of visualisation and charting features that help visual analysis of data and generate insights. From the previously conducted usability review on all ~30 charting features, it was identified that Chart Matrix which lets you chart multiple measures and dimensions in a flexible way could be improved to better serve user jobs. Initially identified issues included:
* Too many functionalities
* Interaction between the feature's colour configuration and main colour configuration is confusing
* Legend keys are missing
* Some of the functionalities behave differently from other visualisation and charting features in the product

I've jumped on in-depth investigation to make the case and plan for the development.

#### Process


**1. Conducted a focus group interview to understand user expectations and pain points**

I've invited 5 users who have data analysis background, the user type which this feature is targeting at. The interview was carried out around the following questions:

1. How do you use it?
   * What are the functionalities you use frequently and rarely?
   * What are the typical steps you follow to build a chart?
   * Do you use all inner label options and size by options?
   * How do you use colour configuration for this feature?
2. What would make this feature more useful – potential use cases?
   * Improve clarity in control panel?
   * Eliminate or hide some of the advanced options?
   * Add other useful features?


**2. Based on interviews formed hypotheses and possible required actions**

![](https://s3.eu-west-2.amazonaws.com/lubynoel-portfolio/chart-matrix-hypotheses.png)

**3. Designed a user survey to validate hypotheses and inform decisions**

The survey was structured into three parts with open feedback at the end:
* Part 1. Product experience and expertise
* Part 2. Interpretation of charting outputs
* Part 3. Use of each of functionality

#### Some of the key findings from the survey

* 70% of the respondents said they rarely use this feature or never used it, main reasons include "not sure when to use it", "hard to interpret", "hard to configure", "not presentable to client"
* Respondents struggled to comprehend the output correctly, i.e. what each element represents - too many values/ aggregates to process at once
* Average score for the chart interpretation test is 4.4 out of 7, i.e. 63% accuracy. No noticeable difference found between roles and expertise level
* Respondents said they find it hard to configure what they want both in values and formatting
* Only 30% respondents were able to correctly how colour buckets work, and many didn’t see the use case for it
* ‘Size by’ is the least understood feature.
80% didn't understand how it works and 70% said they won't use it. 60% couldn't explain what the size of the segment represent

#### Results: Revamped and re-launched the feature

With better understanding of the user jobs and their feedback on the feature, we've revamped the Chart Matrix feature and it became easier to use and produces more presentable outputs.

* Removed some of the advanced technical options that were misleading and/or rarely used
* Instead added new functions that would benefit users, such as ability to control axis, different sorting options
* Improved control panel so it guides a user through the steps to build a chart
