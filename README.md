# Excel Data Analysis Project: Maven Roasters Coffee Shop Sales Analysis

Sales analysis of Maven Roasters' three NYC locations (Hell’s Kitchen, Astoria, and Lower Manhattan) using transactional data from January to June 2023. Includes a dynamic Excel dashboard and actionable insights to optimize operations, boost sales, and improve customer engagement.





## Maven Roasters Sales Analysis

### Overview
Maven Roasters, a fictitious coffee shop chain, operates in  three locations in New York: Hell’s Kitchen, Astoria, and Lower Manhattan. This project analyzes transactional data from January to June 2023 to uncover sales trends, identify peak times, and understand customer preferences.
#### Goals:
- Transform the sales data into a dynamic dashboard. 
- Identify trends and patterns in sales data.
- Determine peak transaction periods and product preferences.
- Develop actionable strategies to improve sales and customer satisfaction.
#### Outcome:
The analysis resulted in a dynamic Excel dashboard and actionable recommendations to support franchise owners in strategic decision-making. Key insights about customer behavior and product preferences are as follows:

[PIC dash]


### Key Highlights

- **Revenue Growth**:
    - Consistent upward trend across all locations, with significant growth in ***March*** and ***May***.
    - A decline in sales was noticed in ***February***.
  
- **Peak Hours and Days**: Transactions peak during morning hours (especialy between 8–11 AM) across all locations, with notable differences in the busiest days:
    - **Hell’s Kitchen**: ***Friday*** sees the highest customer activity.
    - **Astoria**: ***Thursday*** is the most popular day.
    - **Lower Manhattan**: ***Monday*** leads in transactions.
      
- **Top Products**:
    - **Barista Espresso**: The top revenue generator across all locations, particularly popular in ***Hell’s Kitchen*** (revenue collected: ***$ 32,420.20***) and ***Lower Manhattan*** (revenue collected: ***$ 31,051.00***).
    - **Brewed Chai Tea**: Shows significant popularity in ***Astoria***, reflecting customer preference for moderate-caffeine options in that area.
---

### Table of Contents
1. [Dataset Description](#dataset-description)
2. [Analysis Questions](#analysis-questions)
3. [Findings by Location](#findings-by-location)
   - [Hell's Kitchen](#hell's-kitchen)
   - [Astoria](#astoria)
   - [Lower Manhattan](#lower-manhattan)
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
  - `Month`: Derived using **SWITCH** and **MONTH** functions. 
  - `Day`: Derived using **SWITCH** and **WEEKDAY** functions.
  - `Hour`:  Created using the **HOUR** function.
- **Data Quality**:
  - No missing values or inconsistencies.
  - Clean and ready for analysis.




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
- **Daily and Hourly Insights**:

    - `High Traffic on Fridays`: Reflects increased customer activity aligning with end-of-week routines.
    - `Weekend Preference`: Sunday outperforms weekdays like Monday, Wednesday, and Thursday, highlighting a strong customer preference for weekend visits.
    - `Peak Hours`: Occur between 8 AM and 11 AM, driven by commuter traffic and early coffee seekers.
    - `Post-11 AM Sales Decline`: Sales decline sharply after 11 AM but remain steady through 8 PM.
    - `Evening Sales Drop`: Sales drop significantly after 8 PM, likely due to reduced interest in hot beverages and customers exploring other dining options.
- **Product Performance Insights**:
  
    - `High-Caffeine Preference`: Customers tend to prefer high-caffeine-content espresso-based beverages like Barista Espresso.
    - `Moderate-Caffeine Preference`: There is a significant preference for moderate-caffeine beverages like Brewed Chai Tea.
    - `Bakery Pairing`: The popularity of bakery items, especially scones, shows that customers like to pair their beverages with baked goods.
    - `Non-Caffeinated Options`: Hot chocolate’s popularity indicates that customers also prefer non-caffeinated options.
    - `Syrup Flavours`: More customers tend to prefer regular syrup flavours over sugar-free ones. 
    - `Take-Home Products`: Customers show less interest in take-home products like coffee beans, loose tea, packaged chocolate, and branded items.

---

### **Astoria**
[Astoria transaction by day.png]
- **Top Transaction Day**: Thursday (7,427 transactions)
- **Top Transaction Hour**: 10–11 AM
- **Top Product**: Brewed Chai Tea (6,293 transactions)
- **Daily and Hourly Insights**:
  
  - Midweek Spike: High Thursday transactions reflect a midweek spike in caffeine demand.
  - Lower Saturday and Tuesday Visits: Fewer customers visit the coffee shop on Saturdays and Tuesdays compared to other days.
  - Weekend Trends: Weekend caffeine demand is lower as customers explore other food options and activities, though more customers visit on Sundays compared to Saturdays.
  - Morning Dominance: Sales dominate in the mornings (7 AM–11 AM), indicating high commuter activity.
  - Steady Evening Flow: Steady customer flow all day with consistent evening activity, likely due to residents and professionals returning from work.
    
- **Product Performance Insights**:
  
  - `Moderate-Caffeine Preference`: Customers favor moderate-caffeine beverages like Brewed Chai Tea over high-caffeine options like Barista Espresso.
  - `Non-Caffeinated Options`: The popularity of hot chocolate shows that customers also enjoy non-caffeinated options.
  - `Bakery Popularity`: People prefer pairing scones with their beverages, making them more popular than pastries and biscotti, similar to the trend in Hell's Kitchen.
  - `Syrup Flavors`: More customers prefer regular syrup flavors over sugar-free ones.
  - `Take-Home Products`: Customers show less interest in take-home products such as coffee beans, loose tea, packaged chocolate, and branded items.


---

### **Lower Manhattan**
- **Top Transaction Day**: Monday (7,136 transactions)
- **Top Transaction Hour**: 7–10 AM
- **Top Product**: Barista Espresso ($31,051 revenue)
- **Daily and Hourly Insights**:

  - `Monday Visits`: Most customers visit on Mondays, likely for a caffeine boost or a quick grab on their way to work.
  - `Midweek Spikes`: Midweek spikes in transactions, similar to the trend in Astoria, are probably due to client meetings.
  - `Weekend Decrease`: Weekend transactions decrease due to lower demand and less foot traffic.
  - `Morning Dominance`: Most customers visit before 11 AM, with sales dropping by 60.52% afterward, likely due to low caffeine demand and limited food options.
  - `Evening Decline`: Decreasing sales after 4 PM and very few sales after 7 PM show minimal foot traffic and low interest in hot beverages during evening hours.
    
- **Product Performance Insights**:

  - `Caffeine Preferences`: Customers prefer high-to-moderate caffeine drinks like Barista Espresso, Gourmet Brewed Coffee, and Brewed Chai Tea. Black and herbal teas are also popular.
  - `Bakery Pairing`: The popularity of bakery items, especially scones, indicates that customers enjoy pairing their beverages with baked goods(similar trend to Astoria and Hell's Kitchen).
  - `Hot Chocolate Appeal`: Hot chocolate, though less popular (comapred to the trend in Astoria and Hell's Kitchen), generated ***$ 22.4k***, appealing to tourists, children, and families.
  - `Syrup Flavors`: Regular syrup flavors are preferred over sugar-free ones.
  - `Take-Home Products`: Customers show less interest in take-home products like coffee beans, loose tea, packaged chocolate, and branded items.

---

## Comparative Summary

| Metric                  | Hell’s Kitchen       | Astoria            | Lower Manhattan    |
|-------------------------|----------------------|--------------------|--------------------|
| **Top Transaction Day** | Friday               | Thursday           | Monday             |
| **Top Hour**            | 8 AM - 11 AM        | 10 AM - 11 AM      | 7 AM - 10 AM       |
| **Top Product**         | Barista Espresso    | Brewed Chai Tea    | Barista Espresso   |
| **Evening Activity**    | Consistent till 8 PM| Consistent till 8 PM| Declines post 5 PM |

---

### **Recommendations**

- `Address February Decline`:
    - Launch **Valentine’s-themed** beverages and bakery items.
    - Introduce **limited-edition** branded chocolates and **Valentine's-themed** merchandise.

- `Seasonal Menu`:
    - Promote **limited edition iced beverages and summer special snacks** during the summer.
    - Roll out festive drinks like ***Pumpkin Spice Latte*** during the fall and ***Peppermint Mocha*** during the holidays.

- `Weekend Offers`:
    - Introduce **“happy family combo”** on weekends to attract tourists and families.
    - Offer **loyalty points** for **word-of-mouth referrals** to friends.

- `Customer Surveys`: Conduct surveys regularly to understand **customer preferences** and modify the menu accordingly.

- `Expand Menu`:
    - **Introduce grab-and-go customizable “all-day sandwiches” and “lunch wraps”** to boost sales, especially post-11am.
    - **Add healthy options** like fresh salads and soup to your lunch and dinner menu.
    - **Add non-caffeinated beverages** (smoothies, milkshakes, fruit juices, or flavored water) to attract families and children.

- `Leverage Delivery Services`:
    - **Partner with Uber Eats or DoorDash** to enhance accessibility especially in Lower Manhattan.

- `Host Events to Boost Coffee Beans and Tea Leaves`:
    - **Host coffee-tea workshops** to boost brand engagement and sales.
    - **Offer loyalty rewards** for workshop referrals.

- `Expand Merchandise`:
    - **Offer affordable daily-use items** like tote bags, reusable coffee sleeves, stickers, and notepads.
    - **Introduce festive/limited edition local-themed mugs and t-shirts** to build brand loyalty.

- `Website or App`: **Launch smartphone-based apps** for pre-ordering and customizing food, reducing morning wait times.

- `Closing Time`:
    - **Lower Manhattan**:
        - Close early due to minimal foot traffic after 7pm.
        - Focus on quick service, lunch, and delivery options for working professionals.
        - Conduct surveys to understand customer needs before extending hours past 7pm.
    - **Maintain the same business hours** in Astoria and Hell’s Kitchen.



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



