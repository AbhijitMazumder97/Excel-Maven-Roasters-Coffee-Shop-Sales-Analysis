# Coffee Shop Sales Analysis

## Project Overview
**Maven Roasters**, a fictitious coffee shop chain, operating at three locations in **New York: Hell’s Kitchen, Astoria, and Lower Manhattan**. This project analyzes **transactional data from January to June 2023** to **uncover sales trends, identify peak times, and understand customer preferences**.

### Goals
- **Transform** the sales data into a dynamic dashboard. 
- **Identify** trends and patterns in sales data.
- **Determine** peak transaction periods and product preferences.
- **Develop** actionable strategies to improve sales and customer satisfaction.

### Outcome
The analysis resulted in a **dynamic Excel dashboard and actionable recommendations** to support franchise owners in strategic decision-making. A short video clip of the dashboard visual is attached below for reference. [View Excel Dashboard](https://view.officeapps.live.com/op/view.aspx?src=https%3A%2F%2Fraw.githubusercontent.com%2FAbhijitMazumder97%2FExcel-Maven-Roasters-Coffee-Shop-Sales-Analysis%2Frefs%2Fheads%2Fmain%2FMAVEN%2520ANALYTICS%2520COFFEE%2520SHOP%2520SALES%2520GUIDED%2520PROJECT.xlsx&wdOrigin=BROWSELINK)

https://github.com/user-attachments/assets/fe91cf09-af3a-4012-967e-3dfc53ce8d16


## Key Insights

- **${\color{brown}\text{Revenue Growth}}$**
    - Consistent increasing trend across all locations, with significant growth in ***March*** and ***May***.
    - A decline in sales in ***February***.
  
- **${\color{brown}\text{Peak Hours and Days}}$**
Transactions peak during morning hours **(especialy between 8–11 AM) across all locations** due to **high commuter activity**, with notable differences in the busiest days:

    - `Hell’s Kitchen:` ***Friday*** sees the highest activity.
    - `Astoria:` ***Thursday*** is the most popular day.
    - `Lower Manhattan:` ***Monday*** leads in transactions.
      
- **${\color{brown}\text{Top Products}}$**
    - **Barista Espresso**: The **top revenue generator** across all locations, particularly **popular** in ***Hell’s Kitchen*** (revenue collected: ***$ 32,420.20***) and ***Lower Manhattan*** (revenue collected: ***$ 31,051.00***).
    - **Brewed Chai Tea**: Shows **significant popularity** in ***Astoria***, reflecting customer preference for **moderate-caffeine options** in that area.
---

## Contents
1. [Dataset Description](#dataset-description)
2. [Analysis Questions](#analysis-questions)
3. [Revenue Insights Across All Locations](#revenue-insights-across-all-locations)
4. [Location-Specific Insights](#location-specific-insights)
   - [Hell's Kitchen](#hells-kitchen)
   - [Astoria](#astoria)
   - [Lower Manhattan](#lower-manhattan)
5. [Comparative Summary](#comparative-summary)
6. [Recommendations](#recommendations)
   - [Valentine's Week Specials](#valentines-week-specials)
   - [Weekend Workshops](#weekend-workshops)
   - [Expand Menu](#expand-menu)
   - [Optimize Operational Efficiency](#optimize-operational-efficiency)
   - [Expand Merchandise](#expand-merchandise)
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
- **${\color{brown}\text{High Revenue Generating Product:}}$** Barista Espresso ($32,420 revenue)
- **${\color{brown}\text{Popular Product:}}$** Barista Espresso (6153 transactions)

- **${\color{brown}\text{Daily and Hourly Insights:}}$**
![hkhourlydailytrans](https://github.com/user-attachments/assets/6ab3e4d7-6b3b-42c1-9671-cfa579de1702)

    - `High Traffic on Fridays`: Reflects **increased customer activity** aligning with **end-of-week routines**.
    - `Weekend Preference`: **Sunday outperforms** weekdays like Monday, Wednesday, and Thursday, highlighting a **strong customer preference for weekend visits**.
    - `Peak Hours`: Between **8 AM and 11 AM**, driven by **commuter traffic and early coffee seekers**.
    - `Sales Decline`: **Sharp decline** in sales after 11 AM but **remain steady** through 8 PM.
    - `Evening Sales Drop`: Sales drop significantly after 8 PM, likely due to **reduced interest in hot beverages and customers exploring other dining options**.

  




> [!Note]
> ${\color{#051094}\text{Each column in "Transactions by hour" column chart visual represents an entire hour duration. Eg. 7 means between 7AM and 8AM.}}$
${\color{#051094}\text{Total number of transactions that occurred between 7AM and 8AM from January 2023 to June 2023 was 3455 in Hell's Kitchen.}}$



- **${\color{brown}\text{Product Performance Insights:}}$**
![hkproductperformance](https://github.com/user-attachments/assets/438e8ffd-f70c-4d2c-90ff-ed99ec2a04d4)


    - `High-Caffeine Preference`: Customers tend to prefer **high-caffeine-content espresso-based beverages** like Barista Espresso.
    - `Moderate-Caffeine Preference`: There is a significant preference for **moderate-caffeine beverages** like Brewed Chai Tea.
    - `Bakery Pairing`: The popularity of bakery items, **especially scones**, shows that customers like to pair their beverages with baked goods.
    - `Non-Caffeinated Options`: **Hot chocolate’s** popularity indicates that customers also prefer **non-caffeinated options**.
    - `Syrup Flavours`: More customers tend to **prefer regular syrup flavours** over sugar-free ones. 
    - `Take-Home Products and packaged items`: **Strong Preference for fresh products** as customers are **less interested** in take-home products and packaged items like ***coffee beans, loose tea, packaged chocolate, and branded items***.



---

### **Astoria**



- **${\color{brown}\text{Top Transaction Day:}}$** Thursday (7,427 transactions)
- **${\color{brown}\text{Top Transaction Hours:}}$** 7–11 AM
- **${\color{brown}\text{High Revenue Generating Product:}}$** Barista Espresso ($27,427.90 revenue)
- **${\color{brown}\text{Popular Product:}}$** Brewed Chai Tea (6,293 transactions)

  
- **${\color{brown}\text{Daily and Hourly Insights:}}$**

 ![ashourlydailytrans](https://github.com/user-attachments/assets/83d9525d-59e4-444f-a6f2-c2cf1ea74d73)


  - `Midweek Spike`: High Thursday transactions reflect a midweek spike in caffeine demand. **Increasing Mid-week caffeine** demand probably driven by **residents taking breaks** from their daily routine and **remote working professionals** combating **work fatigue**.
  - `Lower Saturday and Tuesday Visits`: **Less caffeine demand** on Tuesdays and Saturdays indicating customers are exploring other options like **Taco Tuesdays** or **Saturday-special Brunch-Dinner** options.
  - `Weekend Trends`: Weekend caffeine demand is **lower as customers explore other food options and activities**, though **more customers visit on Sundays** compared to Saturdays.
  - `Morning Dominance`: Sales **dominate in the morning hours (7 AM–11 AM)**, indicating **high commuter activity**.
  - `Steady Evening Flow`: Steady customer flow all day with **consistent evening activity**, likely due to **residents and professionals returning from work**.
    
- **${\color{brown}\text{Product Performance Insights:}}$**
  
  
![astoria_product_performance](https://github.com/user-attachments/assets/00699db5-7f4d-4dbb-a37d-4091b197ed0c)

 
  - `Moderate-Caffeine Preference`: Customers **favor moderate-caffeine beverages like Brewed Chai Tea** over high-caffeine options like Barista Espresso.
  - `Non-Caffeinated Options`: The popularity of **hot chocolate** shows that **customers also enjoy non-caffeinated options**.
  - `Bakery Popularity`: **Scones are strongly preferred** among other bakery options like pastries and biscotti, **similar to the trend in Hell's Kitchen**.
  - `Syrup Flavors`: **Preference for regular syrup flavors** over sugar-free ones.
  - `Take-Home and Packaged Products`: Customers show **less interest** in take-home products such as coffee beans, loose tea, packaged chocolate, and branded items.


---

### **Lower Manhattan**

- **${\color{brown}\text{Top Transaction Day:}}$**  Monday (7,136 transactions)
- **${\color{brown}\text{Top Transaction Hours:}}$** 7–11 AM
- **${\color{brown}\text{High Revenue Generating Product:}}$** Barista Espresso ($31,051 revenue)
- **${\color{brown}\text{Popular Product:}}$** Barista Espresso (5320 transactions)

- **${\color{brown}\text{Daily and Hourly Insights:}}$**
![lmdailyhourlytrans](https://github.com/user-attachments/assets/27c0e5fe-bd98-4d4d-b593-1ef8dedbf383)


  - `Monday Visits`: **Most customers** visit on Mondays, likely for a **early-week caffeine boost or a quick grab on their way to work**.
  - `Midweek Spikes`: Midweek spikes in transactions, similar to the trend in Astoria, are probably due to **client meetings or professionals fighting work fatigue**.
  - `Weekend Decrease`: Weekend transactions decrease due to **lower demand and less foot traffic**.
  - `Morning Dominance`: Most customers **visit before 11 AM**, with sales **dropping heavily afterward**, likely due to **low caffeine demand and limited food options**.
  - `Evening Decline`: Decreasing sales after 4 PM and **very few sales after 7 PM** show **minimal foot traffic** and **low interest** in hot beverages during evening hours.
    
- **${\color{brown}\text{Product Performance Insights:}}$**

![lmproductperformance](https://github.com/user-attachments/assets/fd696ddd-8522-4a66-96ed-4d20ff169d9b)



  - `Caffeine Preferences`: **Customers prefer high-to-moderate caffeine options** like Barista Espresso, Gourmet Brewed Coffee, and Brewed Chai Tea **probably to boost their productivity**. Black and herbal teas are also popular.
  - `Bakery Pairing`: **Scones** are a popular beverage pairing option(**similar to the trend in Astoria and Hell's Kitchen**).
  - `Hot Chocolate Appeal`: **Hot chocolate**, though **less popular** (compared to the trend in Astoria and Hell's Kitchen), generated ***$ 22.4k***, **appealing to tourists, children, and families**.
  - `Syrup Flavors`: Regular syrup flavors **are preferred** over sugar-free ones.
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


> [!Note]
> **${\color{#051094}\text{"Average Transactions Before 11 AM" is the average number of the transactions occuring every hour before 11 AM.}}$**
**${\color{#051094}\text{Similarly, "Average Transactions After 11 AM" is the average number of the transactions occuring every hour after 11 AM.}}$**
**$${\color{#051094} \text{Average Decrease Post 11 AM} = \left( \frac{\text{Average Transactions Before 11 AM} - \text{Average Transactions After 11 AM}}{\text{Average Transactions Before 11 AM}} \right) \times 100 }$$**



**${\color{brown}\text{Key Insights:}}$**
  - `February Drop`: Astoria showed the maximum sales decline, as **residential customers prioritized essential needs over discretionary items** due to post-holiday fatigue and colder weather.
  - `Post-11 AM Sales`: Lower Manhattan experienced a **sharp decline in sales after 11 AM, driven by limited lunch options**.
  - `Midweek Activity`: Thursdays are consistently active across all regions, reflecting **growing caffeine demand midweek**.
  - `Evening Activity`: Astoria and Hell’s Kitchen maintain **steady evening sales until 8 PM**, unlike Lower Manhattan, where **sales drop significantly after 4 PM**.
  - `Weekend Activity`: **Weekends see lower activity overall**, with Saturdays least active in Hell’s Kitchen and Astoria, and Sundays least active in Lower Manhattan.


---

## **Recommendations**

#### **Valentine's Week Specials**

Launch **limited-edition Valentine’s-themed branded items** and **special beverages** during Valentine's Week to address February Decline.

- `Limited Edition Branded Items`:

  - **Valentine's themed T-shirt:** $20 each.
          ![newDALL·E 2024-12-11 19 23 59 - A relaxed-fit white T-shirt with a natural, slightly wrinkled texture, featuring the text I ❤️️ my coffee in bold black font with a red heart symbol (1)](https://github.com/user-attachments/assets/90bfa969-1c2f-4174-b86c-49caaf9b7c02)
          ![newDALL·E 2024-12-11 19 23 59 - A relaxed-fit white T-shirt with a natural, slightly wrinkled texture, featuring the text I ❤️️ my coffee in bold black font with a red heart symbol (](https://github.com/user-attachments/assets/7d04653e-aacc-4d72-b30d-cb522e21563a)

  - **Beverage Sleeves (neoprene sleeves):** $12 each.
          ![new maven roasters coffee cup sleeve](https://github.com/user-attachments/assets/5d549a56-949d-4e70-922f-2c3c64bbecbf)

      - `Valentine’s Special Beverages`:

        - **Chocolate Covered Strawberry Mocha:** $8 each.
              ![chocolate-covered-strawberry-mocha](https://github.com/user-attachments/assets/c7f91357-d303-4acd-9f58-d4fff366cb1d)

        - **Raspberry White Chocolate Cappuccino:** $9 each.
          ![new1020-white-chocolate-raspberry-cappuccino-1020](https://github.com/user-attachments/assets/cff6ed68-bb15-4ac8-a7f9-726a65261028)

#### **Weekend Workshops**
Start Weekend Workshops to boost the **Coffee Beans and Loose Tea sales**.

- Organize **paid weekend workshops ($25-$30 per head)** to **spread awareness** about sourcing of **Coffee Beans/Loose Tea** and their preparation methods.
- Offer **group discounts** for participants registering with three or more friends.
- Provide **loyalty rewards** for referrals and returning participants.
- Introduce **special bundle offers on coffee beans and tea leaves** for all participants.
- Conduct **online campaigns** for promotions and **special discounts** on online purchases during **winter season**.

![small_pexels-shkrabaanthony-7176003](https://github.com/user-attachments/assets/2111e282-f4f3-4d4d-8a72-bf126cec99d2)

Photo by Antoni Shkraba: https://www.pexels.com/photo/people-making-coffee-in-filter-at-cafe-kitchen-7176003/


#### **Expand Menu**
Add new **quick grab and go** food/beverage options to your menu to mitigate the sales drop post 11 AM.

- `Cold Beverages:` Introduce **cold beverages options under $5-$6**, like iced chai lattes, frozen chai, iced lattes, iced coffee, frozen hot chocolate, and smoothies.

- `Lunch Combo:` Introduce **lunch combo under $15**:
    - **Customizable sandwiches** with veg, non-veg and vegan options.
    - Any **beverage** of choice (hot/cold)
          
- `Food Delivery:` **Partner with Uber Eats or DoorDash** to enhance accessibility especially in Lower Manhattan.

![pexels-felipe-vieira-651921657-20066369](https://github.com/user-attachments/assets/361d77e7-ba3c-4cd4-8bf6-cbc5d73c778a)

Photo by Felipe Vieira: https://www.pexels.com/photo/sandwich-and-beverage-20066369/

    
#### **Optimize Operational Efficiency**
    
- `Closing Time:`
    - **Close early in Lower Manhattan** due to **minimal foot traffic** after 7 pm.
    - **Conduct surveys** to **understand customer needs** before extending hours past 7 pm.
    - Maintain the **same business hours** in Astoria and Hell’s Kitchen.

![pexels-timmossholder-28726700](https://github.com/user-attachments/assets/4ebaaf9e-6f07-481d-b7c0-ecde34fc7240)

Photo by Tim Mossholder: https://www.pexels.com/photo/closed-sign-hanging-on-storefront-window-28726700/

- `Streamlining Operations:`
    - Launch **smartphone apps** for **pre-ordering and customizing food** to reduce morning wait times.
    - Ensure **sufficient staff members** during busy morning hours.
    - Assign **specific staff for pre-orders** during **peak times** and **others for walk-in customers**.
    - Set up **separate counters** for pre-order and walk-in customers to reduce wait times.
    - Allow customers to choose a **pick-up time** and **send notifications** when the **order is ready to ensure freshness**.

![pexels-pavel-danilyuk-6612738](https://github.com/user-attachments/assets/8b7fbc28-c34f-4e6b-bc3a-1203fb93b025)

Photo by Pavel Danilyuk: https://www.pexels.com/photo/a-woman-standing-behind-the-counter-of-a-coffee-shop-6612738/


#### **Expand Merchandise:**

- Launch **affordable daily-use items** like tote bags, and notepads.

![9568a9f02c1c8207cbff66c7d6e265e9](https://github.com/user-attachments/assets/a962f652-9d07-48f4-8ea3-80b610770103)
      
- Partner with **local artists** and introduce **local themed** T-shirts, mugs and hoodies.

![local themed merchandise](https://github.com/user-attachments/assets/688e737a-2dc9-43cd-a203-6852fb00a3eb)


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
This analysis provides valuable insights into **customer behavior** at Maven Roasters. By implementing the recommendations, the Maven Roasters are expected to achieve an **18% increase** in February revenue, a **19% improvement** in post-11 AM transactions, a **21.5% growth** in coffee bean sales, and a **10.5%** rise in loose tea sales. Additionally, operational efficiency is projected to **improve by 8.5%**, driving overall sales growth and customer satisfaction.[recommendation impact.pdf](https://github.com/user-attachments/files/18202772/recommendation.impact.pdf)




