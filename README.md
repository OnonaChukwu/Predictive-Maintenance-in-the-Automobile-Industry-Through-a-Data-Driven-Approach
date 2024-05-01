# Predictive Maintenance in the Automobile Industry Through a Data-Driven Approach

## Introduction
- The automobile industry seeks to maintain vehicle reliability while minimizing costs and downtime.

![image](https://github.com/OnonaChukwu/Predictive_maintenance/assets/155753951/b83f65d5-bff8-4614-a5b3-451bd4ebc1c9)

- Predictive maintenance through utilizing a data-driven approach for pre-emptive maintenance planning can mitigate it.

## Project Goal
- To harness detailed vehicle data to forecast maintenance needs and enable proactive maintenance strategies.

## Objectives
- To analyze the impact of vehicle characteristics on maintenance requirements.
- To assess the role of operational factors in predictive maintenance outcomes.

## Key Questions
- How do age and mileage affect maintenance frequency and critical failures?
- What is the impact of vehicle usage on repair costs and number of repairs?
- What differences in maintenance needs between engine types exist?
- Correlation between warning signals and severity of maintenance required.
- Relationship between the time since last maintenance and vehicle's maintenance/repair history.
  
![image](https://github.com/OnonaChukwu/Predictive_maintenance/assets/155753951/9d15d8c2-3b93-44ec-b1ea-c21aa32dc699)

## Data Description
- Data comprises details from a fleet of vehicles, including maintenance frequency, engine type, repair costs, critical failures, and more.
- Data is anonymized and generated to reflect realistic automotive industry scenarios, as was confirmed through online checks.

## Methodology
- Employed exploratory data analysis (EDA) and predictive modeling to identify patterns and predict maintenance needs.
- Tools used include Python with pandas, matplotlib, and scikit-learn, along with data generation in Excel.

## Results 
**Question 1**: How do the age and mileage of a vehicle affect its maintenance frequency and the likelihood of critical failures?

![image](https://github.com/OnonaChukwu/Predictive_maintenance/assets/155753951/6647c6ef-b46a-45f7-b155-988d5e3b5776)

- Weak correlations exist between these variables! In fact, they are almost negligible.
- This implies that: age, mileage, maintenance frequency, critical failures do not impact each other.

**Question 2**: What is the impact of vehicle usage (personal vs. commercial) on the average repair cost and the number of repairs?

![image](https://github.com/OnonaChukwu/Predictive_maintenance/assets/155753951/1e24a775-c23d-4f78-8c21-c881ddf16ce8) 

![image](https://github.com/OnonaChukwu/Predictive_maintenance/assets/155753951/b7fbac93-b56a-4bfb-baf4-a9f47ba79416)

- Commercial vehicles cost less (769Eur) compared to private (788Eur), but the frequency of repair in private (4.42) is slightly lower compared to commercial (4.50).
- For owners and operators, understanding these differences can inform budgeting for maintenance costs. 
- Businesses using commercial vehicles may anticipate more frequent repairs but can also expect slightly lower costs per repair. 
- In contrast, private users might face repairs less frequently but with a higher cost per instance. 
- These emphasize on the importance of long-term preventive maintenance and budget planning.

**Question 3**. Are there significant differences in maintenance needs and costs between different engine types (e.g., Petrol, diesel, electric, hybrid)?

 ![image](https://github.com/OnonaChukwu/Predictive_maintenance/assets/155753951/0cdae313-80b4-484d-8092-0dfda859bf62)
 
 ![image](https://github.com/OnonaChukwu/Predictive_maintenance/assets/155753951/394d4308-6c69-41f1-af6b-28d72b7bb757)
 
- Diesel and electric engine vehicles exhibit lower maintenance frequencies but incur slightly higher repair costs, with electric engines being the most expensive to repair. 
- Hybrid engines, despite requiring the most frequent maintenance, benefit from the lowest average repair costs, which suggests efficient repair management.
- Petrol engines maintain a middle ground, with a maintenance frequency and repair cost that are neither the highest nor the lowest. 
- Overall, the choice of engine type influences both the frequency of maintenance required and the associated repair costs; this highlights the trade-offs between different vehicle technologies.

**Question 4**: Can the number of warning signals before maintenance predict the severity of maintenance required or the occurrence of critical failures?
- The correlation coefficient of 0.013499 between Warning Signals Count and Critical Failures suggests a very weak positive linear relationship.
- It indicates that warning signals do not influence critical failures.

**Question 5**: How does the time elapsed since the last maintenance (days since last maintenance) correlate with the vehicle's overall maintenance and repair history (including costs and critical failures)?

![image](https://github.com/OnonaChukwu/Predictive_maintenance/assets/155753951/551005ab-314b-4ade-98dc-2c2aab9758c8)  

![image](https://github.com/OnonaChukwu/Predictive_maintenance/assets/155753951/adbf1655-ef5e-4ab9-967f-92bdedb93eae)

- The correlation matrix indicates that Days Since Last Maintenance has a very weak negative correlation with Critical Failures (-0.008281);
   - almost no relationship exists between them.
- Additionally, there is a very weak positive correlation between Days Since Last Maintenance and Average Repair Cost (0.003552).
- Another still weak positive correlation between Critical Failures and Average Repair Cost (0.027415).

## The Take-Home Key Analysis and Insights
- Minor correlations between vehicle age, mileage, and maintenance frequency or critical failures.
- Commercial usage tends to have slightly lower average repair costs but more frequent repairs than personal usage.
- Maintenance needs and costs vary minimally across engine types, with hybrid engines having slightly higher frequency but lower costs.
- A weak correlation exists between the number of warning signals and the occurrence of critical failures.
- No strong correlation between days since last maintenance and critical failures or repair costs.

## Conclusions
- Predictive maintenance can be tailored based on vehicle usage, age, and engine type, though differences are not stark for this very project.
- Warning signals and time since last maintenance offer limited predictive value for critical failures or maintenance costs.
- Engine type and vehicle usage influence maintenance frequency and costs to a certain extent.

## Recommendations
- Focus on developing more nuanced predictive models that consider a combination of factors, rather than relying on single metrics.
- Enhance data collection on operational metrics for more accurate predictions, including real-time monitoring and historical analysis.
- Implement targeted maintenance strategies based on vehicle usage patterns and engine types to optimize maintenance schedules and reduce unnecessary expenditures.
