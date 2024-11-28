# Excel Data Analysis Project: Maven Roasters Coffee Shop Sales Analysis

Sales analysis of Maven Roasters' three NYC locations (Hell’s Kitchen, Astoria, and Lower Manhattan) using transactional data from January to June 2023. Includes a dynamic Excel dashboard and actionable insights to optimize operations, boost sales, and improve customer engagement.





# Maven Roasters Sales Analysis

## Overview
Maven Roasters, a fictitious coffee shop chain, operates in  three locations in New York: Hell’s Kitchen, Astoria, and Lower Manhattan. This project analyzes transactional data from January to June 2023 to uncover sales trends, identify peak times, and understand customer preferences.
#### Goals:
- Transform the sales data into a dynamic dashboard. 
- Identify trends and patterns in sales data.
- Determine peak transaction periods and product preferences.
- Develop actionable strategies to improve sales and customer satisfaction.



## Key Highlights
- **Revenue Growth**: Consistent upward trend across locations, with significant growth in March and May.
- **Peak Hours**: Mornings (7–11 AM) dominate transactions across all locations.
- **Top Products**: Barista Espresso leads revenue generation, while Brewed Chai Tea is most popular in Astoria.

---

## Table of Contents
1. [Dataset Description](#dataset-description)
2. [Analysis Questions](#analysis-questions)
3. [Findings by Location](#findings-by-location)
4. [Comparative Summary](#comparative-summary)
5. [Recommendations](#recommendations)
6. [Technical Skills Used](#technical-skills-used)
7. [Dashboard Preview](#dashboard-preview)
8. [Conclusion](#conclusion)

---

## Dataset Description
- **Timeframe**: January 2023 – June 2023
- **Volume**: 149,456 rows, 11 fields
- **Calculated Columns**:
  - `Revenue`: Transaction quantity × Unit price.
  - `Month`, `Day`, `Hour`: Extracted using Excel formulas (`SWITCH`,`MONTH` ,`HOUR`, `WEEKDAY`).

---

## Analysis Questions
1. How have sales trended over time?
2. Which days and hours drive the most transactions?
3. Which products are most/least popular? Which drive the most revenue?

---

## Findings by Location

### **Hell’s Kitchen**

- **Top Transaction Day**: Friday (7,489 transactions)
- **Top Transaction Hour**: 8–11 AM
- **Top Product**: Barista Espresso ($32,420 revenue)
- **Insights**:
  - High traffic on Fridays reflects increased customer activity aligning with end-of-week routines.
  - Sunday outperforms weekdays such as Monday, Wednesday, and Thursday, highlighting a strong customer preference for weekend visits.
  - Peak hours occur between 8 AM and 11 AM, driven by commuter traffic and early coffee seekers.
  - Sales decline sharply after 11 AM but remain steady through 8 PM.
  - Sales drop significantly after 8 PM, likely due to reduced interest in hot beverages and customers exploring other dining options.

---

### **Astoria**
- **Top Transaction Day**: Thursday (7,427 transactions)
- **Top Transaction Hour**: 10–11 AM
- **Top Product**: Brewed Chai Tea (6,293 transactions)
- **Insights**:
  - Strong midweek demand for caffeine.
  - Evening activity suggests professionals returning from work.

---

### **Lower Manhattan**
- **Top Transaction Day**: Monday (7,136 transactions)
- **Top Transaction Hour**: 7–10 AM
- **Top Product**: Barista Espresso ($31,051 revenue)
- **Insights**:
  - High Monday sales reflect caffeine needs at the start of the week.
  - Minimal activity post-7 PM due to reduced foot traffic.

---

## Comparative Summary

| Metric                  | Hell’s Kitchen       | Astoria            | Lower Manhattan    |
|-------------------------|----------------------|--------------------|--------------------|
| **Top Transaction Day** | Friday               | Thursday           | Monday             |
| **Top Hour**            | 8 AM - 11 AM        | 10 AM - 11 AM      | 7 AM - 10 AM       |
| **Top Product**         | Barista Espresso    | Brewed Chai Tea    | Barista Espresso   |
| **Evening Activity**    | Consistent till 8 PM| Consistent till 8 PM| Declines post 5 PM |

---

## Recommendations

### **Location-Specific Strategies**
1. **Hell’s Kitchen**:
   - Offer Friday morning promotions targeting commuters.
   - Introduce loyalty programs for morning customers.

2. **Astoria**:
   - Promote Brewed Chai Tea and family-friendly combos on Sundays.
   - Leverage evening foot traffic with meal-and-drink bundles.

3. **Lower Manhattan**:
   - Focus on Monday deals for repeat customers.
   - Close earlier post-7 PM and prioritize delivery options for professionals.

### **General Strategies**
- Launch Valentine-themed beverages in February to boost sales.
- Expand the menu with grab-and-go lunch options (e.g., sandwiches, wraps, salads).
- Partner with delivery services like Uber Eats to capture lunch and evening customers.
- Develop a loyalty program to reward frequent visitors and referrals.

---

## Technical Skills Used
- **Tools**: Microsoft Excel
- **Techniques**: Pivot Tables, calculated columns (`SWITCH`,`MONTH` ,`WEEKDAY`, `HOUR` functions)
- **Visualization**: Line charts, bar graphs, and dashboards for insights presentation.

---

## Dashboard Preview
![Dashboard Screenshot](path/to/dashboard-image.png)

---

## Conclusion
This analysis provides valuable insights into customer behavior and operational performance at Maven Roasters. By implementing the recommendations, the company can increase revenue, enhance customer satisfaction, and improve operational efficiency.

