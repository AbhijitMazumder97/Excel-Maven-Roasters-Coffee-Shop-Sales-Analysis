# Coffee Shop Sales Analysis

## Project Overview
**Maven Roasters**, a fictitious coffee shop chain, operating at three locations in **New York: Hell’s Kitchen, Astoria, and Lower Manhattan**. This project analyzes **transactional data from January to June 2023** to **uncover sales trends, identify peak times, and understand customer preferences**.

### Goals
- **Transform** the sales data into a dynamic dashboard. 
- **Identify** trends and patterns in sales data.
- **Determine** peak transaction periods and product preferences.
- **Develop** actionable strategies to improve sales and customer satisfaction.

### Outcome
The analysis resulted in a **dynamic Excel dashboard and actionable recommendations** to support franchise owners in strategic decision-making. A short video clip of the dashboard visual is attached below for refference:

https://github.com/user-attachments/assets/fe91cf09-af3a-4012-967e-3dfc53ce8d16


## Key Highlights

- **${\color{brown}\text{Revenue Growth}}$**
    - Consistent increasing trend across all locations, with significant growth in ***March*** and ***May***.
    - A decline in sales in ***February***.
  
- **${\color{brown}\text{Peak Hours and Days}}$**
Transactions peak during morning hours **(especialy between 8–11 AM) across all locations** due to **high commuter activity**, with notable differences in the busiest days:

    - **Hell’s Kitchen**: ***Friday*** sees the highest customer activity.
    - **Astoria**: ***Thursday*** is the most popular day.
    - **Lower Manhattan**: ***Monday*** leads in transactions.
      
- **${\color{brown}\text{Top Products}}$**
    - **Barista Espresso**: The top revenue generator across all locations, particularly popular in ***Hell’s Kitchen*** (revenue collected: ***$ 32,420.20***) and ***Lower Manhattan*** (revenue collected: ***$ 31,051.00***).
    - **Brewed Chai Tea**: Shows significant popularity in ***Astoria***, reflecting customer preference for **moderate-caffeine options** in that area.
---

## Table of Contents
1. [Dataset Description](#dataset-description)
2. [Analysis Questions](#analysis-questions)
3. [Revenue Insights Across All Locations](#revenue-insights-across-all-locations)
4. [Location-Specific Insights](#location-specific-insights)
   - [Hell's Kitchen](#hells-kitchen)
   - [Astoria](#astoria)
   - [Lower Manhattan](#lower-manhattan)
5. [Comparative Summary](#comparative-summary)
6. [Recommendations](#recommendations)
7. [Technical Skills Used](#technical-skills-used)
8. [Conclusion](#conclusion)

---

## Dataset Description

![data desc](https://github.com/user-attachments/assets/58520e66-ddcc-4827-a043-43d3813bd688)
![dataset](https://github.com/user-attachments/assets/fe0d4e2a-4ed1-4a93-a2e7-d3a8bbe067b2)


- **${\color{brown}\text{Timeframe}}$**: January 2023 – June 2023
- **${\color{brown}\text{Volume}}$**: 149,456 rows, 11 fields
- **${\color{brown}\text{Calculated Columns}}$**:
  - `Revenue`: Transaction quantity × Unit price.
  - `Month`: Derived using **SWITCH** and **MONTH** functions.
    ![screenshotmonth](https://github.com/user-attachments/assets/cdbbfc33-93af-4392-b526-3021321f6890)

  - `Day`: Derived using **SWITCH** and **WEEKDAY** functions.
    ![screenday](https://github.com/user-attachments/assets/61e7e710-cc11-423b-b762-995fbcf70014)

  - `Hour`:  Created using the **HOUR** function.
- **${\color{brown}\text{Data Quality}}$**:
  - No missing values or inconsistencies.
  - Clean and ready for analysis.
---

## Analysis Questions
1. How have sales trended over time?
2. Which days and hours drive the most transactions?
3. Which products are most/least popular? Which drive the most revenue?

---
## Revenue Insights Across All Locations: 
${\color{blue}\text{(common to all three locations)}}$


![arevenue](https://github.com/user-attachments/assets/e111521d-e424-4cd3-b5d5-31ac5c9d89a7)
${\color{brown}\text{Fig.: Astoria Revenue Trend}}$

![hkrevenue](https://github.com/user-attachments/assets/687fe19f-058b-4f9c-a200-732596ca0162)
${\color{brown}\text{Fig.: Hell's Kitchen Revenue Trend}}$

![lmrevenue](https://github.com/user-attachments/assets/f10b687e-c22e-47f9-8a47-8f83ce10dec5)
${\color{brown}\text{Fig.: Lower Manhattan Revenue Trend}}$


- **February** saw a decline due to post-holiday fatigue or cold weather.
- Strong revenue growth from **March to May (maximum growth in May)** reflects high spring caffeine demand and increased customer traffic.
- Minimal growth in **June** suggests stabilization, highlighting the need for targeted summer promotions.

## Location-Specific Insights

### **Hell’s Kitchen**

- **${\color{brown}\text{Top Transaction Day:}}$** Friday (7,489 transactions)
- **${\color{brown}\text{Top Transaction Hours:}}$** 8–11 AM
- **${\color{brown}\text{Top Product:}}$** Barista Espresso ($32,420 revenue)

- **${\color{brown}\text{Daily and Hourly Insights:}}$**
  
    - `High Traffic on Fridays`: Reflects **increased customer activity** aligning with **end-of-week routines**.
    - `Weekend Preference`: **Sunday outperforms** weekdays like Monday, Wednesday, and Thursday, highlighting a **strong customer preference for weekend visits**.
    - `Peak Hours`: Occur between **8 AM and 11 AM**, driven by **commuter traffic and early coffee seekers**.
    - `Sales Decline`: Sales decline sharply after 11 AM but remain steady through 8 PM.
    - `Evening Sales Drop`: Sales drop significantly after 8 PM, likely due to **reduced interest in hot beverages and customers exploring other dining options**.

  
![hkhourlydailytrans](https://github.com/user-attachments/assets/6ab3e4d7-6b3b-42c1-9671-cfa579de1702)
${\color{brown}\text{Fig.: Hell's Kitchen daily and hourly transactions}}$


  


${\color{red}\text{Note: Each column in "Transactions by hour" visual represents an entire hour duration. Eg. 7 means between 7AM and 8AM.}}$
${\color{red}\text{Total number of transactions that occurred between 7AM and 8AM from January 2023 to June 2023 was 3455 in Hell's Kitchen.}}$


- **${\color{brown}\text{Product Performance Insights:}}$**
 
    - `High-Caffeine Preference`: Customers tend to prefer **high-caffeine-content espresso-based beverages** like Barista Espresso.
    - `Moderate-Caffeine Preference`: There is a significant preference for **moderate-caffeine beverages** like Brewed Chai Tea.
    - `Bakery Pairing`: The popularity of bakery items, especially scones, shows that customers like to pair their beverages with baked goods.
    - `Non-Caffeinated Options`: **Hot chocolate’s** popularity indicates that customers also prefer **non-caffeinated options**.
    - `Syrup Flavours`: More customers tend to **prefer regular syrup flavours** over sugar-free ones. 
    - `Take-Home Products and packaged items`: Customers show **less interest in take-home products and packaged items** like coffee beans, loose tea, packaged chocolate, and branded items. **Strong Preference for fresh products**.

![hkproductperformance](https://github.com/user-attachments/assets/438e8ffd-f70c-4d2c-90ff-ed99ec2a04d4)

${\color{brown}\text{Fig.: Hell's Kitchen product performance and revenue}}$


---

### **Astoria**



- **${\color{brown}\text{Top Transaction Day:}}$** Thursday (7,427 transactions)
- **${\color{brown}\text{Top Transaction Hours:}}$** 7–11 AM
- **${\color{brown}\text{Top Product:}}$** Brewed Chai Tea (6,293 transactions)

  
- **${\color{brown}\text{Daily and Hourly Insights:}}$**

 ![ashourlydailytrans](https://github.com/user-attachments/assets/83d9525d-59e4-444f-a6f2-c2cf1ea74d73)
${\color{brown}\text{Fig.: Astoria daily and hourly transactions}}$

  - `Midweek Spike`: High Thursday transactions reflect a midweek spike in caffeine demand. **Increasing Mid-week caffeine** demand probably driven by **residents taking breaks from their daily routine and remote working professionals combating work fatigue**.
  - `Lower Saturday and Tuesday Visits`: **Less caffeine demand** on Tuesdays and Saturdays indicating customers are exploring other options like **Taco Tuesdays** or **Saturday-special Brunch-Dinner** options.
  - `Weekend Trends`: Weekend caffeine demand is **lower as customers explore other food options and activities**, though **more customers visit on Sundays** compared to Saturdays.
  - `Morning Dominance`: Sales **dominate in the morning hours (7 AM–11 AM)**, indicating **high commuter activity**.
  - `Steady Evening Flow`: Steady customer flow all day with **consistent evening activity**, likely due to **residents and professionals returning from work**.
    
- **${\color{brown}\text{Product Performance Insights:}}$**
  
  
![astoria_product_performance](https://github.com/user-attachments/assets/00699db5-7f4d-4dbb-a37d-4091b197ed0c)

  ${\color{brown}\text{Fig.: Astoria product performance and revenue}}$

  - `Moderate-Caffeine Preference`: Customers **favor moderate-caffeine beverages like Brewed Chai Tea** over high-caffeine options like Barista Espresso.
  - `Non-Caffeinated Options`: The popularity of **hot chocolate** shows that **customers also enjoy non-caffeinated options**.
  - `Bakery Popularity`: People prefer pairing bakery with their beverages. **Scones are strongly preferred** among other bakery options like pastries and biscotti, **similar to the trend in Hell's Kitchen**.
  - `Syrup Flavors`: **Preference for regular syrup flavors** over sugar-free ones.
  - `Take-Home and Packaged Products`: Customers show **less interest** in take-home products such as coffee beans, loose tea, packaged chocolate, and branded items.


---

### **Lower Manhattan**

- **${\color{brown}\text{Top Transaction Day:}}$**  Monday (7,136 transactions)
- **${\color{brown}\text{Top Transaction Hours:}}$** 7–11 AM
- **${\color{brown}\text{Top Product:}}$** Barista Espresso ($31,051 revenue)

- **${\color{brown}\text{Daily and Hourly Insights:}}$**
![lmdailyhourlytrans](https://github.com/user-attachments/assets/27c0e5fe-bd98-4d4d-b593-1ef8dedbf383)
${\color{brown}\text{Fig.: Lower Manhattan daily and hourly transactions}}$

  - `Monday Visits`: Most customers visit on Mondays, likely for a **early-week caffeine boost or a quick grab on their way to work**.
  - `Midweek Spikes`: Midweek spikes in transactions, similar to the trend in Astoria, are probably due to **client meetings or professionals fighting work fatigue**.
  - `Weekend Decrease`: Weekend transactions decrease due to **lower demand and less foot traffic**.
  - `Morning Dominance`: Most customers **visit before 11 AM, with sales dropping heavily afterward**, likely due to **low caffeine demand and limited food options**.
  - `Evening Decline`: Decreasing sales after 4 PM and **very few sales after 7 PM show minimal foot traffic and low interest in hot beverages during evening hours**.
    
- **${\color{brown}\text{Product Performance Insights:}}$**

![lmproductperformance](https://github.com/user-attachments/assets/fd696ddd-8522-4a66-96ed-4d20ff169d9b)

${\color{brown}\text{Fig.: Lower Manhattan product performance and revenue}}$

  - `Caffeine Preferences`: **Customers prefer high-to-moderate caffeine options** like Barista Espresso, Gourmet Brewed Coffee, and Brewed Chai Tea **probably to boost their productivity**. Black and herbal teas are also popular.
  - `Bakery Pairing`: **Scones** are a popular beverage pairing option(**similar to the trend in Astoria and Hell's Kitchen**).
  - `Hot Chocolate Appeal`: **Hot chocolate**, though **less popular** (compared to the trend in Astoria and Hell's Kitchen), generated ***$ 22.4k***, **appealing to tourists, children, and families**.
  - `Syrup Flavors`: Regular syrup flavors are preferred over sugar-free ones.
  - `Take-Home Products`: Customers **prefer fresh food items** over **packaged and take-home products** like coffee beans, loose tea, packaged chocolate, and branded items.

---

## Comparative Summary

| **Metric**                  | **Hell’s Kitchen**                              | **Astoria**                                   | **Lower Manhattan**                          |
|-----------------------------|-----------------------------------------------|---------------------------------------------|---------------------------------------------|
| **Least Transaction Day**   | Saturday                                       | Saturday                                    | Sunday                                      |
| **Top Transaction Day**     | Friday                                         | Thursday                                    | Monday                                      |
| **Peak Hours**              | 8 AM - 11 AM                                   | 7 AM - 11 AM                                | 7 AM - 11 AM                                |
| **Evening Activity**        | Consistent evening activity till 8 PM experiencing a sharp decrease afterward.         | Consistent activity till 8 PM.              | Sales decreasing post-5 PM. Very few sales post-7 PM. |
| **Midweek Activity**        | Sales increased from Thursdays after experiencing a drop on Wednesdays reaching peak on Friday.   | Sales increased from Wednesdays and reached its peak on Thursdays after facing a decline on Tuesdays.        | Midweek spike in sales on Thursdays.        |
| **Top Product**             | Barista Espresso                               | Brewed Chai Tea                             | Barista Espresso                            |
| **Least Popular Product**   | Branded Items (119 transactions)               | Packaged Chocolate (110 transactions)       | Packaged Chocolate (180 transactions)       |
| **Drinking Chocolate Popularity** | 4th rank (3763 transactions)                | 4th rank (4300 transactions)                | 7th rank (3405 transactions)                |
| **February Sales Drop**           | 7.55%                                         | 8.09%                                       | 4.61%                                       |
| **Spring Performance (March-May)** | Total Revenue: $126,013.64<br>Max revenue increase: May (30.51%) | Total Revenue: $124,741.80<br>Max revenue increase: May (32.81%) | Total Revenue: $123,748.08<br>Max revenue increase: May (32.02%) |
| **Average Transactions Before 11 AM** | 5152.8                                      | 4880.25                                     | 5340                                       |
| **Average Transactions After 11 AM**  | 2497.10                                     | 3453.11                                     | 2108.20                                    |
| **Average Decrease Post 11 AM** | 51.54%                                       | 29.24%                                     | 60.52%                                     |


**${\color{red}\text{Note:
"Average Transactions Before 11 AM" is the average number of the transactions occuring every hour before 11 AM.}}$**
**${\color{red}\text{Similarly, "Average Transactions After 11 AM" is the average number of the transactions occuring every hour after 11 AM.}}$**
**$${\color{red} \text{Average Decrease Post 11 AM} = \left( \frac{\text{Average Transactions Before 11 AM} - \text{Average Transactions After 11 AM}}{\text{Average Transactions Before 11 AM}} \right) \times 100 }$$**



**${\color{brown}\text{Key Insights:}}$**
  - `February Drop`: Astoria showed the maximum sales decline, as **residential customers prioritized essential needs over discretionary items** due to post-holiday fatigue and colder weather.
  - `Post-11 AM Sales`: Lower Manhattan experienced a **sharp decline in sales after 11 AM, driven by limited lunch options**.
  - `Midweek Activity`: Thursdays are consistently active across all regions, reflecting **growing caffeine demand midweek**.
  - `Evening Activity`: Astoria and Hell’s Kitchen maintain **steady evening sales until 8 PM**, unlike Lower Manhattan, where **sales drop significantly after 4 PM**.
  - `Weekend Activity`: **Weekends see lower activity overall**, with Saturdays least active in Hell’s Kitchen and Astoria, and Sundays least active in Lower Manhattan.


---

## **Recommendations**

- **${\color{brown}\text{Address February Decline:}}$**
  
    - Leverage **Valentine's Week** and launch **special Valentine’s-themed** beverages, **limited-edition** branded chocolates, bakery items and **Valentine's-themed** merchandise to boost sales.
    - Offer **limited time offer discounts** on **coffee beans and tea leaves** encouraging customers especially in residential areas to enjoy their coffee/tea from the comfort of their home.
    - Offer **loyalty options** for instore shopping during the winter months like February.

![Red-velvet-latte-2](https://github.com/user-attachments/assets/83d30269-a1af-46ac-b376-c026cf050893)

**${\color{brown}\text{Fig: Red Velvet Latte}}$**
      

- **${\color{brown}\text{ Weekend Workshops and special offers:}}$**
    - **Host weekend coffee-tea workshops** to educate customers and boost coffee-bean and Tea leaves sales.
    - Introduce **“happy family combo”** on weekends to attract tourists and families.
    - Offer **loyalty points** for **word-of-mouth referrals** to friends.
      
![small_pexels-shkrabaanthony-7176003](https://github.com/user-attachments/assets/2111e282-f4f3-4d4d-8a72-bf126cec99d2)

Photo by Antoni Shkraba: https://www.pexels.com/photo/people-making-coffee-in-filter-at-cafe-kitchen-7176003/
**${\color{brown}\text{Fig: Coffee workshop}}$**
   
 

- **${\color{brown}\text{Expand Menu:}}$**
    - Introduce grab-and-go customizable **all-day sandwiches and lunch wraps** to boost sales, especially post-11am.
![Grilled_Chicken](https://github.com/user-attachments/assets/bc5c5f28-2fa1-417e-97dd-abcb8d18b7df)
**${\color{brown}\text{Fig: Grilled chicken sandwich paired with iced Tea}}$**

    - Add **healthy options** like fresh salads and soup to your lunch and dinner menu.
    - **Add non-caffeinated iced beverages** (smoothies, milkshakes, fruit juices, or flavored water) to attract families and children.
![4459682](https://github.com/user-attachments/assets/64df472b-fd86-4488-9dd7-c09208d89dd3)
**${\color{brown}\text{Fig: Vanilla Milkshake}}$**
      
    - Introduce a rotating seasonal menu and promote **limited edition iced beverages and summer special snacks** during the summer.

  ![pexels-cottonbro-4790062](https://github.com/user-attachments/assets/1fe1ed2f-731f-47e4-8a5b-473b55eb2d35)

  Photo by cottonbro studio: https://www.pexels.com/photo/ice-cream-in-clear-drinking-glass-4790062/
     **${\color{brown}\text{Fig: Iced Summer Beverages}}$**
      
    - Roll out festive drinks like ***Pumpkin Spice Latte*** during the fall and ***Peppermint Mocha*** during the holidays.
![holiday and fall](https://github.com/user-attachments/assets/5fc09dc0-be19-455d-9d79-79fea5cea4e2)
**${\color{brown}\text{Fig: Peppermint Mocha (Right) and Pumpkin Spice Latte (Left)}}$**

    - **Conduct surveys** regularly to understand **customer preferences** and modify the menu accordingly.
    - **Partner with Uber Eats or DoorDash** to enhance accessibility especially in Lower Manhattan.

- **${\color{brown}\text{Expand Merchandise:}}$**
    - Offer affordable daily-use items like **tote bags, reusable coffee sleeves, stickers, and notepads**.
    - Introduce **festive/limited edition local-themed mugs, t-shirts or hoodies** to build brand loyalty.
      
    ![coffee cup sleeve](https://github.com/user-attachments/assets/a90cfa63-412c-4d28-995e-fc8d5ebf9f62)

    **${\color{brown}\text{Fig: Reusable Coffee cup sleeves}}$**
      
    ![9568a9f02c1c8207cbff66c7d6e265e9](https://github.com/user-attachments/assets/a962f652-9d07-48f4-8ea3-80b610770103)

    **${\color{brown}\text{Fig: Tote bags}}$**
      
    ![local themed merchandise](https://github.com/user-attachments/assets/688e737a-2dc9-43cd-a203-6852fb00a3eb)

    **${\color{brown}\text{Fig: Astoria themed Hellgate Bridge Hoodie}}$**


- **${\color{brown}\text{Gift-Chocolates:}}$**
  
    - Market chocolates as **gift items** by improving packaging (e.g., gift boxes, ribbons).
    - Promote **seasonal offerings** (e.g., holiday-themed chocolates).
    - Conduct **taste events and surveys** to understand customer preferences.
      
    ![19897962_fpx](https://github.com/user-attachments/assets/aa431ce0-a067-41db-9da7-00988ad1e1ad)

    **${\color{brown}\text{Fig: Chocolate Gift box}}$**
    
- **${\color{brown}\text{Closing Time and operational efficiency:}}$**
    - **Lower Manhattan**:
        - **Close early** due to minimal foot traffic **after 7pm**.
        - Focus on **quick service, lunch, and delivery options** for working professionals.
        - Conduct **surveys** to understand customer needs before extending hours past 7pm.
    - **Maintain the same business hours** in Astoria and Hell’s Kitchen.
    - **Launch smartphone-based apps** for pre-ordering and customizing food, reducing morning wait times.
    - Ensure there are **sufficient staff members** to handle the rush, particularly during busy morning hours.



---

## Technical Skills Used
- **${\color{brown}\text{Tools:}}$**: Microsoft Excel
- **${\color{brown}\text{Techniques and Visualization:}}$**
    - `Calculated columns` : Derived calculated columns like **Revenue, Day, Hour, and Month using functions SWITCH, MONTH, WEEKDAY and HOUR**.
    -  `Conditional formatting`: Used the conditional formatting feature to highlight the **Revenue** column in the top 15 product types pivot table, ensuring **darker shades highlight high revenue** and **lighter shades highlight lower revenue figures**.
    - `Line charts`: Used to feature the **revenue growth trend**.
    - `Bar graphs`: Used to feature **daily, hourly sales and popular product categories**.
    - `Slicers`: Used a slicer with buttons for Hell's Kitchen, Lower Manhattan and Astoria to **filter and analyze data** specific to these locations.
    - `Pivot Tables`: Used to feature the **top 15 product types**.
---

## Conclusion
This analysis provides valuable insights into customer behavior and operational performance at Maven Roasters. By implementing the recommendations, the company can increase revenue, enhance customer satisfaction, and improve operational efficiency.



