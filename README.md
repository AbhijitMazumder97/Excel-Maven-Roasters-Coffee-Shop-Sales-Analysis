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
  
  - `Midweek Spike`: High Thursday transactions reflect a midweek spike in caffeine demand.
  - `Lower Saturday and Tuesday Visits`: Less customers showed up on Tuesdays and Saturdays indicating less caffeine demand on these day. Customers are exploring other options like **Taco Tuesdays** or **Saturday-special Brunch** menus.
  - `Weekend Trends`: Weekend caffeine demand is lower as customers explore other food options and activities, though more customers visit on Sundays compared to Saturdays.
  - `Morning Dominance`: Sales dominate in the mornings (7 AM–11 AM), indicating high commuter activity.
  - `Steady Evening Flow`: Steady customer flow all day with consistent evening activity, likely due to residents and professionals returning from work.
    
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

| **Metric**                  | **Hell’s Kitchen**                              | **Astoria**                                   | **Lower Manhattan**                          |
|-----------------------------|-----------------------------------------------|---------------------------------------------|---------------------------------------------|
| **Least Transaction Day**   | Saturday                                       | Saturday                                    | Sunday                                      |
| **Top Transaction Day**     | Friday                                         | Thursday                                    | Monday                                      |
| **Peak Hours**              | 8 AM - 11 AM                                   | 7 AM - 11 AM                                | 7 AM - 11 AM                                |
| **Evening Activity**        | Consistent evening activity till 8 PM.         | Consistent activity till 8 PM.              | Sales decreasing post-5 PM. Very few sales post-7 PM. |
| **Midweek Activity**        | Drop in sales on Wednesdays; peak on Friday.   | Midweek spike in sales on Thursdays.        | Midweek spike in sales on Thursdays.        |
| **Top Product**             | Barista Espresso                               | Brewed Chai Tea                             | Barista Espresso                            |
| **Least Popular Product**   | Branded Items (119 transactions)               | Packaged Chocolate (110 transactions)       | Packaged Chocolate (180 transactions)       |
| **Drinking Chocolate Popularity** | 4th rank (3763 transactions)                | 4th rank (4300 transactions)                | 7th rank (3405 transactions)                |
| **February Drop**           | 7.55%                                         | 8.09%                                       | 4.61%                                       |
| **Spring Performance (March-May)** | Total Revenue: $126,013.64<br>Max revenue increase: May (30.51%) | Total Revenue: $124,741.80<br>Max revenue increase: May (32.81%) | Total Revenue: $123,748.08<br>Max revenue increase: May (32.02%) |
| **Average Transactions Before 11 AM** | 5152.8                                      | 4880.25                                     | 5340                                       |
| **Average Transactions After 11 AM**  | 2497.10                                     | 3453.11                                     | 2108.20                                    |
| **Average Decrease Post 11 AM** | 51.54%                                       | 29.24%                                     | 60.52%                                     |


- #### Key Insights
    - **Morning Activity**:
        - All locations see the majority of transactions before 11 AM, with the highest activity in Lower Manhattan.
        - Significant drops in sales occur after 11 AM, with Lower Manhattan experiencing the steepest decrease (60.52%).
  
    - **Weekend vs. Weekday Performance**:
        - Hell’s Kitchen and Astoria experience the lowest transactions on Saturdays, while Sunday is least active in Lower Manhattan.
        - Peak transaction days vary: Friday (Hell’s Kitchen), Thursday (Astoria), and Monday (Lower Manhattan).

    - **Product Popularity**:
        - Barista Espresso dominates in Hell’s Kitchen and Lower Manhattan, while Brewed Chai Tea is a favorite in Astoria.
        - Packaged products (e.g., branded items and chocolates) are the least popular across all locations.

    - **Spring Revenue Growth**: All locations show strong performance in spring, with May being the highest revenue month, particularly in Astoria (32.81% growth).


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

- `Host Events and Workshops`:
    - **Host coffee-tea workshops** to boost brand engagement and sales.
    - **Offer loyalty rewards** for workshop referrals.

- `Expand Merchandise`:
    - **Offer affordable daily-use items** like tote bags, reusable coffee sleeves, stickers, and notepads.
    - **Introduce festive/limited edition local-themed mugs and t-shirts** to build brand loyalty.

- `Gift-Chocolates`:
    - Market chocolates as **gift items** by improving packaging (e.g., gift boxes, ribbons).
    - Promote **seasonal offerings** (e.g., holiday-themed chocolates).
    - Conduct **taste events and surveys** to understand customer preferences.

- `App and social media`:
    - **Launch smartphone-based apps** for pre-ordering and customizing food, reducing morning wait times.
    - Ensure there are **sufficient staff members** to handle the rush, particularly during busy morning hours.
    -  Online campaign ads on social media to promote less popular products.

- `Closing Time`:
    - **Lower Manhattan**:
        - **Close early** due to minimal foot traffic **after 7pm**.
        - Focus on **quick service, lunch, and delivery options** for working professionals.
        - Conduct **surveys** to understand customer needs before extending hours past 7pm.
    - **Maintain the same business hours** in Astoria and Hell’s Kitchen.

---

## Technical Skills Used
- **Tools**: Microsoft Excel
- **Techniques and Visualization**:
    - `Calculated columns` : Derived calculated columns like **Revenue, Day, Hour, and Month using functions SWITCH, MONTH, WEEKDAY and HOUR**.
    -  `Conditional formatting`: Used the conditional formatting feature to highlight the **Revenue** column in the top 15 product types pivot table, ensuring **darker shades highlight high revenue** and **lighter shades highlight lower revenue figures**.
    - `Line charts`: Used to feature the **revenue growth trend**.
    - `Bar graphs`: Used to feature **daily, hourly sales and popular product categories**.
    - `Slicers`: Used a slicer with buttons for Hell's Kitchen, Lower Manhattan and Astoria to **filter and analyze data** specific to these locations.
    - `Pivot Tables`: Used to feature the **top 15 product types**.
---

## Dashboard Preview
![Dashboard Screenshot](path/to/dashboard-image.png)

---

## Conclusion
This analysis provides valuable insights into customer behavior and operational performance at Maven Roasters. By implementing the recommendations, the company can increase revenue, enhance customer satisfaction, and improve operational efficiency.



