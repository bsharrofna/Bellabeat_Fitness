# Bellabeat Case Study: How Can a Wellness Technology Company Play It Smart?
**Overview**

This project is part of the Google Data Analytics Capstone case study, focusing on Bellabeat, a high-tech company that creates smart wellness products for women.
As a junior data analyst on the Bellabeat marketing team, the goal is to analyze publicly available Fitbit fitness tracker data to identify user behavior trends and provide data-driven recommendations to improve Bellabeat’s marketing strategy.

**Business Objectives**

Bellabeat aims to better understand how consumers use smart devices and apply these insights to their own products, particularly the Bellabeat app.

**Key Questions:**

1. What are some trends in smart device usage?

2. How could these trends apply to Bellabeat customers?

3. How could these insights help influence Bellabeat’s marketing strategy?


**Analytical Approach**

The analysis follows the Google Data Analytics Process (Ask → Prepare → Process → Analyze → Share → Act):

| Step        | Description                  | Deliverable               |
| ----------- | ---------------------------- | ------------------------- |
| **Ask**     | Define the business problem  | Clear business objectives |
| **Prepare** | Collect and load Fitbit data | Dataset overview          |
| **Process** | Clean and transform data     | Ready-to-analyze dataset  |
| **Analyze** | Explore and visualize        | Trends and insights       |
| **Share**   | Present findings             | Visuals and summaries     |
| **Act**     | Make recommendations         | Action plan for marketing |


**Data Source**

* Dataset: FitBit Fitness Tracker Data (CC0)

* Provider: Mobius, Kaggle Open Data

* Description: Data from 30 Fitbit users (April–May 2016), including:

> Daily activity (steps, calories, distance)

> Hourly steps

> Sleep records

> Weight and BMI data

* License: Public Domain (CC0)

**Tools and Libraries**

* Language: R

* Packages Used:

```
library(tidyverse)
library(dplyr)
library(lubridate)
library(ggplot2)
library(tidyr)
```

**Data Cleaning and Preparation**

1. Converted date/time columns to appropriate formats using lubridate.

2. Removed duplicates and handled missing values.

3. Created new features such as:

* weekday (day of week)

* hour (for hourly steps)

* TotalActiveMinutes

4. Verified data integrity and consistency.

**Key Analyses and Visualizations**

1. Daily Activity Trends: Average steps and calories by weekday.

2. Sleep Analysis: Average sleep duration by day of the week.

3. Hourly Activity Patterns: Steps by hour of day and by weekday.

4. Correlation Analysis: Relationships between steps, calories, and activity intensity.

5. Sedentary Behavior: Patterns and improvement opportunities.


**Insights**

* Most active hours: 7 AM – 7 PM, peaking mid-afternoon.

* Weekday activity is higher than weekend activity, suggesting stronger engagement during workdays.

* Sedentary minutes dominate, providing opportunities for wellness challenges.

* Sleep averages approximately 7 hours per night, indicating room for improvement.

* Steps and calories show a strong positive correlation, reinforcing activity as a key health driver.


**Recommendations for Bellabeat**

| Goal                       | Recommendation                                       |
| -------------------------- | ---------------------------------------------------- |
| Increase user engagement   | Push in-app notifications during peak activity hours |
| Reduce sedentary time      | Introduce hourly movement reminders                  |
| Improve wellness awareness | Weekly insights on sleep versus activity             |
| Drive app adoption         | Gamify activity tracking (badges, streaks)           |
| Target marketing           | Emphasize balance, mindfulness, and daily wellness   |


**Repository Structure**
```
bellabeat-case-study/
│
├── Bellabeat_Case_Study.Rmd        # R Markdown notebook
├── Bellabeat_Case_Study.ipynb      # Kaggle-exported Jupyter version (optional)
├── data/                           # Input CSV files
│   ├── dailyActivity_merged.csv
│   ├── sleepDay_merged.csv
│   ├── hourlySteps_merged.csv
│   └── weightLogInfo_merged.csv
├── output/                         # Generated charts, cleaned data, etc.
│   ├── avg_activity.csv
│   ├── avg_sleep.csv
│   └── figures/
│       ├── steps_by_hour.png
│       ├── avg_steps_weekday.png
│       └── sleep_by_day.png
└── README.md                       # Project documentation
```

**How to Run the Notebook**

1. Clone the repository:

```
git clone https://github.com/<your-username>/bellabeat-case-study.git
cd bellabeat-case-study
```
2. Open Bellabeat_Case_Study.Rmd in RStudio (or upload to Kaggle).

3. Install dependencies:
```
install.packages(c("tidyverse", "lubridate", "ggplot2"))
```
4. Knit or run the notebook to generate all outputs.

**References**

* Google Data Analytics Capstone: Bellabeat Case Study

* Kaggle Dataset: FitBit Fitness Tracker Data (CC0)

* Coursera: Data Analysis with R


Bothainah Sharrofna
Data Analyst | R Enthusiast | Lifelong Learner
Email: bsharrofna@gmail.com

   

