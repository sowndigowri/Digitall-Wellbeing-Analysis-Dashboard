# Digital Wellbeing Analysis Platform

> An interactive Power BI analytics platform for understanding digital usage behavior, identifying distraction patterns, and analyzing wellbeing indicators.


## 📌 Project Overview

AWARE AI – Digital Wellbeing Analysis Platform is a data analytics project developed to understand digital usage behavior, identify potential distraction patterns, and analyze wellbeing-related indicators.

Traditional screen-time reports mainly show how long users spend on their devices. This project goes further by analyzing where digital usage is concentrated, which applications and content categories are associated with higher usage or distraction scores, when digital activity occurs, and how these patterns differ across user groups.

The project uses synthetic data and combines Excel, SQL, Power Query, DAX, and Power BI to transform raw data into an interactive analytical dashboard.

---

## 🎯 Project Objectives

The main objectives of the project are:

- Analyze digital usage behavior across users.
- Understand application usage patterns.
- Analyze usage duration and screen-time indicators.
- Identify distraction patterns using distraction scores.
- Analyze distraction across keywords and content categories.
- Understand distraction patterns across different times of day.
- Compare digital behavior across user groups.
- Analyze sleep and wellbeing indicators.
- Present the analysis through an interactive Power BI dashboard.

---

## 💡 Problem Statement

In today's digital environment, people spend significant amounts of time using smartphones, social media, entertainment, gaming, communication, and other digital applications.

Simply measuring total screen time does not explain where the time is being spent or which digital activities are associated with distraction.

Therefore, the project focuses on analyzing digital behavior at multiple levels, including applications, keywords, content categories, usage duration, time of day, user groups, sleep, and wellbeing indicators.

---

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| Excel | Initial data cleaning and preparation |
| SQL | Database storage and connection to Power BI |
| Power Query | ETL, transformation, and data preparation |
| DAX | Analytical measures and calculations |
| Power BI | Data modeling, visualization, and dashboard development |

---

## 🔄 Project Workflow

The project follows the workflow below:

Synthetic Data  
↓  
Excel Data Cleaning  
↓  
SQL Database  
↓  
SQL → Power BI Connection  
↓  
Power Query ETL  
↓  
Data Modeling  
↓  
DAX Measures  
↓  
Power BI Dashboard  
↓  
Insight Generation

---

## 🧹 Data Preparation

The initial dataset was prepared using Excel before being loaded into the SQL database.

The preparation stage focused on improving data quality and ensuring that the data was suitable for analysis.

The prepared data was then stored in SQL and connected to Power BI.

---

## 🗄️ SQL Database

SQL was used as the database layer for the project.

The SQL database served as the source from which the data was connected to Power BI.

No separate SQL-based analytical query layer was used in the project. The major transformations and analytical calculations were performed within Power Query and Power BI using DAX.

---

## 🔄 Power Query ETL

Power Query Editor was used to perform ETL and data preparation inside Power BI.

The transformation stage included tasks such as:

- Data type validation
- Column preparation
- Data transformation
- Data cleaning
- Structuring data for analysis
- Preparing tables for the Power BI data model

---

## 🧮 DAX Measures

DAX was used to create analytical measures required for the dashboard.

Examples of measures used in the project include:

- Total Users
- Average Screen Time
- Average Usage Duration
- Average Distraction Score
- Total Usage Hours
- High Distraction Activities
- Distraction Activity %
- Wellbeing-related measures

These measures allow dashboard visuals to respond dynamically to filters and selections.

---

## 🗂️ Data Model

The Power BI model contains fact tables, dimension tables, and an application reference table.

### Dimension Tables

- `Dim_User`
- `Dim_Date`

### Fact Tables

- `Fact_PhoneUsage`
- `Fact_Wellbeing`
- `Fact_DigitalUsage`

### Application Table

- `App_Ecosystem`

The model connects user, phone usage, wellbeing, digital usage, application, and date information to support multidimensional analysis.

---

## 📊 Dashboard Structure

The Power BI report contains four main pages.

### 1. Introduction

Provides an overview of the AWARE AI project and its purpose.

### 2. Executive Overview

Provides a high-level view of digital usage and distraction patterns.

The page includes analysis of:

- Total users
- Average screen time
- Distraction score
- Wellbeing indicators
- Screen time and social media time by primary use
- Distraction score by keyword
- Top applications by usage duration
- Content category usage

### 3. Distraction Intelligence

Focuses specifically on digital distraction patterns.

The analysis includes:

- Distraction score by time of day
- Distraction score by burnout risk
- Applications associated with distraction
- Distraction score by content category
- High-distraction activities
- Overall usage indicators

### 4. Wellbeing & User Insights

Focuses on user wellbeing and digital behavior.

The analysis includes:

- Screen time by primary use
- Wellbeing and sleep indicators by user status
- User wellbeing distribution
- Digital usage and wellbeing-related indicators

---

## 🔍 Key Insights

The dashboard provides several analytical observations:

### Digital Usage

Digital activity is distributed across multiple application and content categories, allowing usage behavior to be viewed beyond overall screen time.

### Application Usage

Different applications contribute differently to overall usage duration. The dashboard highlights the applications with the highest recorded usage.

### Distraction

Distraction scores can be analyzed across keywords, applications, content categories, and time-of-day periods.

### Keywords

The keyword analysis highlights differences in average distraction scores across selected digital-content keywords.

### Time of Day

Distraction scores can be compared across morning, afternoon, evening, night, and late-night periods to identify variations in digital activity.

### User Groups

Digital usage and wellbeing indicators vary across different user-status groups, allowing user segments to be compared.

### Wellbeing

The dashboard provides a distribution of users across wellbeing categories and combines wellbeing-related indicators with sleep and digital usage information.

---

## 📸 Dashboard Preview

### Introduction

![Introduction Dashboard](dashboard/01_introduction.png)

### Executive Overview

![Executive Overview](dashboard/02_executive_overview.png)

### Distraction Intelligence

![Distraction Intelligence](dashboard/03_distraction_intelligence.png)

### Wellbeing & User Insights

![Wellbeing & User Insights](dashboard/04_wellbeing_user_insights.png)

---

## 🧩 Project Architecture

```text
                  Synthetic Data
                       │
                       ▼
                 Excel Cleaning
                       │
                       ▼
                  SQL Database
                       │
                       ▼
                Power BI Connection
                       │
                       ▼
                Power Query ETL
                       │
                       ▼
                  Data Modeling
                       │
                       ▼
                    DAX
                       │
                       ▼
               Power BI Dashboard
                       │
                       ▼
                     Insights
