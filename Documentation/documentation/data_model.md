# Power BI Data Model

## Overview

The Power BI data model combines user information, phone usage, wellbeing information, digital activity, application information, and date information.

The model allows the dashboard to analyze digital behavior and wellbeing from multiple perspectives.

---

## Tables in the Model

### Dimension Tables

#### Dim_User

Contains the user key used to identify users within the data model.

#### Dim_Date

Contains date-related information used for time-based analysis.

---

### Fact Tables

#### Fact_PhoneUsage

Contains phone usage and general user-related usage information.

#### Fact_Wellbeing

Contains wellbeing and lifestyle-related information.

#### Fact_DigitalUsage

Contains digital activity, application usage, content, keywords, and distraction-related information.

---

### Application Table

#### App_Ecosystem

Contains application-level information such as category, rating, installs, version, genre, and price.

---

## Relationships

The Power BI model contains relationships between the tables that allow information to flow across the analytical model.

The main relationships visible in the model are:

```text
Dim_User
    │
    │ 1 : 1
    ▼
Fact_PhoneUsage
    │
    │ 1 : 1
    ▼
Fact_Wellbeing
    │
    │ 1 : *
    ▼
Fact_DigitalUsage
    ▲
    │ 1 : *
    │
App_Ecosystem
