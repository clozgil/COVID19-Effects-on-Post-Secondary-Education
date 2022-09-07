# COVID19-Effects-on-Post-Secondary-Education

The Notebook contains links that don't operate on Github. It is recommended to view the project below:
https://nbviewer.org/github/clozgil/COVID19-Effects-on-Post-Secondary-Education/blob/main/COVID-19%20Effects%20on%20Post-Secondary%20Education.ipynb


# Introduction

This project is an analysis on the disruptions in post-secondary education (post-sec ed) caused by the COVID-19 pandemic. The article "Disparities in Disruptions to Postsecondary Education Plans" published by Dr. Ran Liu from the University of Wisconsin-Madison shows the potentially devasting effects on the economy, population, and under-representated minorities should post-sec ed plans be disrupted. For this reason, this project will be an exploration of the population who had their post-sec ed plans disrupted. We will pay close attention to discovering who those individuals are, and what were the various reasons for those disruptions. Finally, we'll construct a few classification models to try and predict those who are most likely to cancel their plans. For the purpose of this project, we will treat post-sec ed  as any kind of instruction after high school graduation whether it be from a college, university, community college, trade school, or other occupational school (such as cosmetology or school of culinary arts).

Even though we do run a few classification models, for a notebook that features some deep learning models I have a project that focuses on predicting whether or not an invidual will leave a company below

https://nbviewer.org/github/clozgil/Employee-Churn-Rate-Analysis-and-Prediction/blob/main/Employee%20Churn%20Rate%20Analysis%20and%20Prediction.ipynb


## Data Sources

The United States Census Bureau began conducting the Household Pulse Survey at the start of the pandemic. Even though the survey has undergone various modifications, it has largely kept the same frame and objective. The Bureau releases a Public Use Data File (PUF) each two weeks, which we will use for this project and can be found below:<br>
https://www.census.gov/programs-surveys/household-pulse-survey/datasets.html


## TimeFrame

Our timeframe will be focused from the survey of week 18 (October 28, 2020) to the survey of week 33 (July 5, 2021). 
The PUF gets released in phases, and even though the survey changes from phase to phase, our goal is to merge as many of them in order to create a longer timeframe. This will enable us to better view trends, which is particularly important since vaccine availability in May 2021 most likely played a role in people's answers to the survey. An additional rationale is that this timeframe most likely covers the periods where post-sec ed plans were made and cancelled.

## Dictionary

For additional information on the data, I recommend reviewing the data dictionary associated with each survey. However, to facilitate the analysis, I will note a few columns of importance:
- TNUM_PS: Number of people in household with post-sec ed plans
- PSCHNG#: Types of changes to post-sec ed plans (data contains 7 different types of changes)
- PSWHYCHG#: Reasons for why there were changes (data contains 9 different types of reasons)

## High Impact Questions
High impact questions drove the direction of this project. Even though the format of the PUF was easy to follow, I tried to develop questions that when answered, might have a significant impact. The idea is to let objectives drive the analysis. Below are a few examples:
- What are the most common changes to post-sec edu?
- Why are post-sec plans changing?
- Who are the people most likely to cancel their post-sec plans?
- What are the most common reasons for why someone would cancel their post-sec plans?
- Does computer and internet availability play a role in the decision to cancel?
- How much impact does a school's decision to remain all virtual have on post-secondary education?
