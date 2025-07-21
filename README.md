## TransBorder Freight Data Analysis Report

### Introduction
 
 #### Overview
Transportation systems are the backbone of modern economies, facilitating the movement of goods, services, and people across cities, states, and nations. They are vital for commerce, tourism, and daily living, directly impacting economic productivity and societal well-being. However, as transportation networks grow in complexity, they face numerous challenges, including safety concerns, inefficiencies, and sustainability issues.

The Bureau of Transportation Statistics (BTS) serves as a vital resource in addressing these challenges by providing comprehensive and reliable data on multiple dimensions of transportation systems. This includes passenger travel, freight movement, safety incidents, infrastructure capacity, and environmental impacts. Such data enables policymakers, transportation agencies, and businesses to make informed decisions to enhance transportation systems for the public good.

#### Project Objectives
The goal of this project is to analyze transborder freight data from the BTS to uncover insights related to the efficiency, safety, and environmental impacts of freight transportation across various modes (road, rail, air, and water). Key objectives include:

- Uncover Freight Movement Patterns: Analyze the movement of freight across different transportation modes, identifying trends in volume, routing, and modes of transportation used across regions and time periods.

- Identify Operational Inefficiencies: Investigate areas where transportation systems may experience inefficiencies, such as congestion points, delays, or underutilized infrastructure, and propose methods to optimize resource use and improve throughput.

- Analyze Environmental Impact: Assess the environmental impact of freight transportation by studying data on emissions, fuel usage, and sustainability metrics across different modes of transportation, and recommend strategies for reducing the carbon footprint of the sector.

- Safety and Risk Assessment: Identify transportation safety incidents related to freight, evaluate their causes and consequences, and suggest recommendations for improving safety protocols.

- Economic Disruptions: Analyze how economic disruptions (e.g., trade patterns, policy changes, or global events) impact freight movements and overall transportation efficiency.

- Provide Data-Driven Recommendations: Based on the analysis, provide actionable recommendations to enhance the performance, sustainability, and safety of the transportation systems that handle cross-border freight.

#### Methodological Framework
The analysis will be conducted using the CRISP-DM methodology (Cross-Industry Standard Process for Data Mining), ensuring a structured, iterative approach that drives valuable business insights and leads to practical recommendations. Data wrangling, visualization, and thorough documentation will be integral to the process to ensure the insights are communicated effectively to stakeholders.

### Methodology
#### Utilizing the CRISP-DM Framework
The CRISP-DM methodology provides a structured approach to data mining projects and consists of six phases: Business Understanding, Data Understanding, Data Preparation, Modeling, Evaluation, and Deployment. For this analysis, we will focus primarily on the first three phases.

### Business Understanding
This phase involves defining the business objectives and translating them into data mining goals. The analytical questions guiding this project are as follows:

- How did freight movement patterns shift from 2020 to 2024?
- What are the monthly patterns of freight movement?
- Which modes are more efficient in terms of value per weight?
- What are the top commodities by freight value and weight?
- Which regions contribute most to freight value and weight?
- How does the freight value vary across U.S. states, Mexican states, and Canadian provinces when analyzed by different trade types?
- What are the most common freight route descriptions used in cross-border transportation with Canada and Mexico from 2020 to 2024?

These questions aim to uncover insights that can help improve efficiency, safety, and sustainability in freight transportation.

### Data Understanding
#### Dataset Overview
The datasets provided by BTS cover freight data from 2020 to 2024, including various metrics such as:

- Transport Modes: Different modes of transportation (road, rail, air, water).
- Freight Volume and Weight: Total volume and weight of freight transported.
- Costs: Freight charges associated with the movement of goods.
- Geographic Data: Origin and destination states or provinces.

#### Data Loading and Inspection
The first step in data understanding is to load and inspect the datasets to become familiar with their structure and contents:

#### Data Inspection
After loading the data, it’s important to inspect it for:

- Missing Values: Determine which columns have missing data and the extent of the missingness.
- Data Types: Check data types to ensure they are appropriate for analysis (e.g., numeric, categorical).

### Data Preparation
Data preparation involves cleaning and transforming the data to make it suitable for analysis. Key steps include:

#### Handling Missing Values
To ensure data integrity, missing values will be replaced with appropriate placeholders:

#### Data Type Conversion
Certain columns may need to be converted to the correct data types, such as converting numerical columns from strings to integers.

#### Deriving New Variables
New variables, such as origin region and route descriptions, will be created to enhance analysis.

### Detailed Interpretation of Visualization Results
1. Total Freight Value by Transport Mode Over Years

Overview: The first chart shows total freight value across different transportation modes from 2020 to 2024.

Key Insights:
- Air Transport: There is a significant increase in total freight value transported by air, peaking around 2023. This suggests that air transport may be increasingly preferred for high-value, time-sensitive goods.
- Other Modes: Other modes like Truck, Rail, and Vessel show relatively stable values, with no significant growth trends. The Pipeline and Mail modes also remained low in comparison to Air.
- Overall Trends: The total freight value shows an upward trend, indicating potential growth in freight activities, possibly due to economic recovery or increased trade.

2. Total Freight Weight by Transport Mode Over Years

Overview: This chart presents the total weight of freight transported by each mode over the same period.

Key Insights:
- Predominance of Trucking: Truck transport consistently carries the most weight, highlighting its essential role in freight logistics. This aligns with the common understanding that trucks are often used for short-distance, flexible deliveries.
- Air Transport: Although air transport has a high value, its weight remains low, confirming that it is typically used for high-value, lightweight cargo rather than bulk goods.
- Stability in Other Modes: Similar to the previous chart, the weight transported by Rail and Vessel is stable and relatively low compared to Truck.

3. Monthly Freight Weight by Transport Mode

Overview: This visualization illustrates the monthly fluctuations in freight weight for different transport modes.

Key Insights:
- Seasonality: There's a noticeable seasonal pattern, particularly in Air and Truck transport, with peaks around certain months. This might correlate with seasonal shopping events or agricultural harvest times.
- Flat Line for Some Modes: For modes like Vessel, the weight transported appears relatively flat, indicating less variability in shipping patterns.

4. Cost-Efficiency by Transport Mode (Value per Unit Weight)

Overview: This chart highlights the cost-efficiency (value per unit weight) of different transport modes.

Key Insights:
- Mail as Outlier: Mail transport has an exceptionally high value per unit weight, indicating that although it carries less weight, it represents a high-value segment, likely due to expedited services.
- Low Value for Other Modes: Most other transport modes have significantly lower values per unit weight, indicating that they are typically used for bulkier, lower-value goods.

5. Top 10 Commodities by Value (2020-2024)

Overview: This visualization ranks the top commodities transported by total value.

Key Insights:
- Dominance of Vehicles: Vehicles are the highest-valued commodity, indicating strong trade in automobiles and related parts.
- Electronics and Machinery: Other high-value items include electronics and machinery, which align with global trade trends focusing on technology and manufacturing.

6. Top 10 Commodities by Weight (2020-2024)

Overview: This chart shows the top commodities transported by total weight.

Key Insights:
- Fuels & Oils: Fuels and oils dominate in weight, reflecting their transportation in bulk, which is typical for energy commodities.
- Agricultural Products: Agricultural products are also likely to be heavy, showing the importance of this sector in freight transport.

7. Top 10 Regions by Freight Value (2020-2024)

Overview: This chart highlights regions contributing the most to freight value.

Key Insights:
- Texas as Leader: Texas significantly leads in freight value, likely due to its size, economic activity, and production hubs.
- Diverse Economic Activities: Other states like Michigan and California also show high value, reflecting diverse economic contributions across the country.

8. Top 10 Regions by Freight Weight (2020-2024)

Overview: Similar to the previous chart, this one ranks regions by total weight transported.

Key Insights:
- Texas and Illinois: Texas and Illinois are prominent in both value and weight, indicating their critical roles in both high-value exports and bulk transport.

9. Freight Value by US State and Trade Type

Overview: This chart provides insights into freight values based on state and trade type.

Key Insights:
- State-Specific Trends: Each state shows different strengths in trade types, providing insights into regional economic structures and trade relationships.

10. Top 20 Most Common Freight Route Descriptions

Overview: This visualization details the most common freight routes.

Key Insights:
- Frequent Routes: Routes from Canada to the US (e.g., US-CA) are among the most common, indicating strong cross-border trade relationships.
- Diverse Trade Patterns: The data reveals a complex network of trade routes, reflecting economic ties between regions.

### Recommendations and Conclusions
#### Recommendations
Based on the analysis of the transborder freight data, the following recommendations can be made to optimize freight transportation and address identified challenges:

1. Enhance Infrastructure Investment
- Road and Air Networks: Given the increasing reliance on trucking and air transport for high-value goods, prioritizing investment in road maintenance and air freight facilities could alleviate congestion and improve delivery speeds.
- Intermodal Facilities: Developing intermodal facilities that facilitate seamless transitions between different transport modes can enhance overall logistics efficiency.
2. Leverage Technology for Efficiency
- Data Analytics: Implement advanced data analytics to monitor freight patterns, optimize routes, and predict demand fluctuations. This can lead to more efficient resource allocation and reduced operational costs.
- Automation and AI: Explore the use of automation in warehousing and logistics processes to increase efficiency and reduce human error, particularly in high-volume operations.

3. Focus on Sustainability
- Emissions Reduction: Implement strategies to reduce emissions in freight transport. This could include investing in cleaner technologies, optimizing routes to minimize fuel consumption, and promoting the use of rail and water transport for bulk goods, which are generally more environmentally friendly.
- Sustainable Practices: Encourage the adoption of sustainable practices among logistics providers, such as using electric or hybrid vehicles and optimizing supply chains to minimize waste.

4. Strengthen Cross-Border Trade Relations
- Customs Efficiency: Streamline customs procedures to facilitate faster processing of goods crossing borders, which can reduce delays and improve overall supply chain efficiency.
- Trade Agreements: Engage in dialogues to enhance trade agreements that facilitate smoother logistics and reduce tariffs on key commodities.

5. Diversify Transport Modes
- Encourage Multi-Modal Transport: Promote the use of multiple transportation modes for different types of cargo to optimize costs and enhance reliability.
- Invest in Emerging Modes: Explore emerging transport options, such as drone delivery for small, high-value items, which can further enhance service offerings.

#### Conclusions
The analysis of transborder freight data has revealed critical insights into the dynamics of freight transportation, highlighting trends in volume, value, and the role of different transport modes. Key findings indicate a growing reliance on air transport for high-value goods and the predominant role of trucking in domestic logistics.

The recommendations provided aim to address current challenges in the freight sector, focusing on enhancing efficiency, sustainability, and cross-border trade relations. By implementing these strategies, stakeholders can improve the overall performance of freight transportation systems, ensuring they meet the demands of a rapidly evolving market.
