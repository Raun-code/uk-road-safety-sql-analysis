
# 🚧 Road Accident Analysis and Prediction Using SQL, Machine Learning & Network Science

This repository contains a comprehensive analytical and predictive study on UK road accident data as part of a data science consultancy project. The project includes SQL database modeling, accident trend analysis, clustering, time series forecasting, and social network analysis — aimed at supporting data-driven policy decisions for improved road safety.

---

## 📘 Exercise 1: SQL Database Design and Query Demonstration

### 📝 Objective

To design a secure, scalable SQL relational database and demonstrate how structured queries can extract actionable insights from road accident datasets.

---

### 🔐 Legal, Technical, and Ethical Considerations

**Key Issues:**

* **Privacy Risks:** Storing names and demographics raises data protection concerns (GDPR, UK Data Protection Act 2018).
* **Ethical Use:** Misuse of data for profiling or discrimination must be prevented.
* **Security Measures:** Prevent data leaks through encryption and role-based access.

**How SQL Helps:**

* **Referential Integrity** via primary and foreign keys
* **Data Normalisation** reduces redundancy
* **Controlled Access** using permission levels
* **Anonymisation** of personally identifiable information

---

### 🗂️ Entity-Relationship (ER) Diagram

A simplified ER diagram includes the core tables and key relationships:

* **`accident`**

* **`vehicle`**

* **`casualty`**

* **`lsoa`**

---

### 💻 SQL Query Demonstrations

#### 🔹 Query 1: Oldest Driver or Rider

#### 🔹 Query 2: Total Vehicles of Type 19

#### 🔹 Query 3: Accidents in Kingston Upon Hull (Sample)

---

## 📗 Exercise 2: Accident Pattern Analysis

### 📝 Objective

To explore **when, where, and under what conditions** road accidents occur using statistical and visual analysis.

---

### 🔹 Time & Day Pattern Analysis

* Accidents peak between **3 PM and 6 PM**
* **Friday and Saturday** show the highest weekly accident counts
* Morning rush hours (7–9 AM) show moderate spikes

### 🔹 Motorbike-Specific Trends

**Vehicle Types Analyzed:**

* Motorcycle ≤125cc
* Motorcycle >125cc ≤500cc
* Motorcycle >500cc

**Findings:**

* High accident occurrence on **weekend evenings**
* Motorcycles >500cc involved more during **rural highway hours**

### 🔹 Pedestrian Accidents

* Peak times: **8–9 AM** and **3–6 PM**
* Most accidents occur on **weekdays**, near schools, crossings, and urban roads

---

## 📙 Exercise 3: Machine Learning & Association Rule Mining

### 📝 Apriori Algorithm – Impact on Accident Severity

**Target Variable:** `accident_severity`
**Frequent Variables Used:**

* Road surface
* Light conditions
* Weather
* Vehicle maneuver

**Top Rule Example:**

```
If [wet road] & [night] → Higher severity
```

**Insight:** Poor lighting and surface conditions are strong predictors of severe accidents.

---

## 📕 Exercise 4: Regional Clustering of Accidents

### 📝 Objective

To uncover geographical patterns in accident density for **Kingston upon Hull**, **Humberside**, and **East Riding of Yorkshire**.

**Clustering Technique:** K-Means
**Features Used:** Location coordinates, accident count, speed limits

**Result:**

* 3 clear clusters emerged:

  * Urban core (dense)
  * Suburban areas (moderate)
  * Rural outskirts (sparse but severe)

---

## 📘 Exercise 5: Time Series Forecasting for Policing Areas

### 📝 Objective

To predict **weekly accident trends** in 3 selected police regions using data from 2017–2019.

**Method Used:** SARIMA (Seasonal ARIMA)

**Selected Forces:**

* Humberside
* Merseyside
* South Yorkshire

**Forecast Insight:**

* Anticipated spike in early summer (June/July)
* Significant drop in December holidays

---

## 📒 Exercise 6: Forecasting Hull LSOAs

### 📝 Objective

To forecast daily accidents in **top 3 Hull LSOAs** for July using data from **January–June 2020**.

**Method:** Facebook Prophet

**LSOAs Identified:**

* Kingston upon Hull 007A
* Kingston upon Hull 004C
* Kingston upon Hull 001B

**Outcome:** All three areas show weekday dominance with a downward trend in late July.

---

## 📔 Exercise 7: Social Network Construction

### 📝 Objective

To construct a **social graph** where:

* **Nodes** = accidents
* **Edges** = shared vehicle or casualty attributes

**Network Stats:**

* Nodes
* Edges
* Density
* Avg Degree

---

## 📓 Exercise 8: Centrality Analysis

### 📝 Objective

To compute **edge betweenness centrality** and assess network influence.

**Result:**

* Right-skewed distribution
* Few edges control majority of the flow in the network
* Top 5% of edges hold structural importance

---

## 📔 Exercise 9: Community Detection

### 📝 Algorithms Used

* **Louvain Method**
* **Girvan-Newman**

**Comparison:**

* **Louvain:** 14 communities detected, more modular
* **Girvan-Newman:** 8 communities, more hierarchical

**Insight:** Louvain better captures dense clusters around urban intersections.

---

## ✅ Summary & Recommendations

### 🔎 Key Insights

* Accidents peak during rush hours and weekends
* Motorbike and pedestrian-related accidents are time-sensitive
* Environment and lighting significantly influence accident severity
* Specific regions show predictable, recurring patterns

---

### 📌 Recommendations to Government Agencies

1. **Increase patrols and awareness in peak hours (3–6 PM, weekends)**
2. **Improve street lighting and road surface in high-severity zones**
3. **Introduce AI-driven early warning systems in urban clusters**
4. **Deploy motorcycle awareness campaigns in suburban corridors**
5. **Leverage time series models for proactive emergency planning**

---

