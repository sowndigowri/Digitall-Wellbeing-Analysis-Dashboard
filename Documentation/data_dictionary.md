# Data Dictionary

This document describes the main tables and fields used in the AWARE AI Digital Wellbeing Analysis Platform.

---

## 1. Dim_User

The user dimension contains the unique user identifier used within the Power BI data model.

| Field | Description |
|---|---|
| User_Key | Unique identifier used to identify users |

---

## 2. Dim_Date

The date dimension supports date-based analysis and filtering.

| Field | Description |
|---|---|
| Date | Calendar date |
| Month | Month associated with the date |
| Year | Year associated with the date |

---

## 3. Fact_PhoneUsage

This table contains general phone usage and user-related usage information.

| Field | Description |
|---|---|
| Age | Age of the user |
| Calls Duration (mins/day) | Daily call duration |
| Data Usage (GB/month) | Monthly mobile data usage |
| E-commerce Spend (INR/month) | Monthly e-commerce spending |
| Gaming Time (hrs/day) | Daily gaming time |
| Gender | Gender category |
| Location | User location |
| Monthly Recharge Cost (INR) | Monthly recharge cost |
| Number of Apps Installed | Number of applications installed |

---

## 4. Fact_Wellbeing

This table contains wellbeing and lifestyle-related indicators.

| Field | Description |
|---|---|
| Age | Age of the user |
| Anxiety Score | Anxiety-related score |
| Burnout Risk | Burnout-risk category |
| Caffeine Intake Cups | Number of caffeine cups consumed |
| Content_Type_Preference | Preferred content type |
| Country | User country |
| Daily_Sleep_Hours | Daily sleep duration |
| Daily_Social_Media_Hours | Daily social media usage |
| Emotional_Fatigue_Score | Emotional fatigue indicator |

---

## 5. Fact_DigitalUsage

This table contains digital activity and distraction-related records.

| Field | Description |
|---|---|
| Record_ID | Unique digital usage record |
| User_ID | User identifier |
| App_Name | Application used |
| Keyword | Keyword associated with the activity |
| Content_Category | Category of digital content |
| Usage_Duration_Minutes | Duration of digital usage |
| Distraction_Score | Distraction-related score |
| Location | Location associated with the activity |
| Date | Date of digital activity |
| Time_of_Day | Time period of digital activity |

---

## 6. App_Ecosystem

This table contains application-level information.

| Field | Description |
|---|---|
| Android_Ver | Android version |
| Category | Application category |
| Content_Rating | Application content rating |
| Current_Ver | Current application version |
| Genres | Application genres |
| Installs | Number of installs |
| Last_Updated | Application last updated date |
| Price_USD | Application price |
| Rating | Application rating |

---

## Purpose of the Data Model

The tables together allow the Power BI dashboard to analyze:

- Digital usage
- Application usage
- Usage duration
- Distraction
- Content categories
- Keywords
- Time of day
- User groups
- Sleep
- Wellbeing

The data model connects these areas so that the dashboard can provide a combined view of digital behavior and wellbeing indicators.
