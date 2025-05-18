# Electric-Vehicle-Sales-Analysis
![Dashboard](https://github.com/user-attachments/assets/f1cb2f05-ba07-4485-8bf5-c36fecd852e9)

## Business Problem
The automotive industry is undergoing a major transformation with the rapid adoption of electric vehicles (EVs), driven by environmental concerns, government incentives, and evolving consumer preferences. However, automotive manufacturers and dealerships face critical challenges in understanding which EV models are performing best, where demand is concentrated geographically, and how battery range affects market eligibility and adoption.

## Business Questions
1. **Which EV manufacturers are leading the market ?**
2. **What is the trend of EV adoption over the years ?**
3. **What is the market share of BEV's vs PHEV's ?**
4. **What is the average electric range of EV's ?**
5. **Which states are leading in EV adoption ?**
6. **Which cities have the highest concentration of PHEV's ?**

---
## Insights 
1. **Eligibility Data Gaps (CAFV Status):**
    A large portion of vehicles (60,613) have unknown CAFV eligibility due to missing battery range data. This limits the ability to         assess the full landscape of clean alternative fuel vehicles.

2. **Geographic Concentration:**
   Washington state dominates with 130,527 vehicles, suggesting either better adoption infrastructure or more complete reporting. Many      other states have negligible counts, pointing to uneven distribution or incomplete data.

3. **Sales Trend Fluctuations:**
   From 2011 to 2018, vehicle sales grew steadily, peaking in 2018. After a dip in 2019, sales rebounded sharply to the highest point in    2023 (30,366 vehicles), followed by a dramatic drop in 2024 (305), likely due to incomplete data reporting.

4. **PHEV Urban Adoption:**
   Seattle stands out with 4,330 Plug-in Hybrid Electric Vehicles (PHEVs), much higher than other cities. Most other cities show a          steady but modest adoption pattern, concentrated in the Washington state area.

## Recommendations

1. **Address Data Incompleteness:**
   Enhance data collection, especially on battery range, to enable more accurate classification of CAFV eligibility and better analysis.

2. **Explore Infrastructure Correlation:**
   Investigate why Washington, particularly Seattle, has high vehicle and PHEV counts—likely factors include charging infrastructure,       local policies, or incentives—and consider replicating these in lower-adoption areas.

3. **Clarify 2024 Sales Drop:**
    Confirm whether the sharp decline in 2024 vehicle sales is due to a reporting lag or actual market disruption. Accurate year-end         data is crucial for trend forecasting.

4. **Promote PHEV Awareness:**
   Cities with moderate PHEV counts could benefit from awareness campaigns or incentives to boost adoption, taking cues from successful     cities like Seattle.

---
## Dataset
[https://github.com/Sujay93/Electric-Vehicle-Sales-Analysis/blob/main/Electric_vehicle_cleaned_data.csv]

## Data cleaning
* Imported the dataset using Python libraries to prepare for analysis.
* Identified and removed duplicates to maintain data accuracy.
* Handled missing values through appropriate replacement strategies to ensure completeness.
* Eliminated irrelevant columns not aligned with the analysis objectives.
* Validated and corrected data types for consistency and analytical accuracy.
* Standardized formatting to enhance data usability for analysis
* Exported the cleaned data set to Tableau for data visualization and analysis.

## Data Visualization and Analysis
1. **Top 10 Vehicles by Make**
![Top 10 Vehicles by make](https://github.com/user-attachments/assets/d99bb464-7962-41a0-8797-b7f6aecc13c7)

* **Tesla Leads the Market:** **With 68,943 vehicles**, Tesla holds a dominant position in the EV market, far surpassing all other         brands.
* **Significant Gap with Contenders:** **Nissan (13,497)** and **Chevrolet (12,025)** trail behind Tesla but remain notable               contributors to EV adoption.
* **Mid-Tier Presence:** Brands like **Ford, BMW, and Kia** form the mid-range segment, each contributing between 6,000–7,600 vehicles.
* **Smaller Market Share:** **Toyota, Volkswagen, Volvo, and Jeep** complete the top 10 with fewer than 6,000 vehicles each,              highlighting a steep drop after the top players.
* **Concentrated Market:** The EV market is highly concentrated, with the top three manufacturers accounting for a majority of total        sales, emphasizing limited brand diversity among leading EV options.

2. **Total Vehicles by CAFV Eligibility**
   ![Total Vehicles by CAFV eligibility](https://github.com/user-attachments/assets/bb6088b6-895e-4b68-9760-dea22f20deb8)

* **Major Data Gap Identified:** **60,613 vehicles have an unknown eligibility status** due to missing battery range data, indicating a   need for improved data collection.
* **Low Battery Range Impact:** **14,287 vehicles** are explicitly marked as ineligible for CAFV benefits due to inadequate battery        range.
* **Skewed Average:** **The average line at 43,608** is heavily influenced by the large volume of unknowns, suggesting the overall         distribution may be distorted.
* **Eligibility Classification Challenge:** The dominance of unclassified vehicles hinders accurate assessment of the market’s CAFV        compliance levels.

3. **Total Vehicles by State**
   ![Total Vehicles by state](https://github.com/user-attachments/assets/d19ccdf4-2d9c-4be4-8638-1bd94c29de84)

* **Washington Dominates:** **Washington (WA) leads with 130,527 vehicles**, far surpassing all other states.
* **Sparse Distribution Elsewhere:** Most states show very low vehicle counts (often fewer than 10), with **California (80), Virginia     (33), and   Maryland (27)** following.
* **Geographic Imbalance:** The Western U.S., particularly WA, shows higher adoption, while Midwestern and Central states lag               significantly.
* **Color coding:** Darker green shades reflect higher vehicle counts, offering a quick visual grasp of regional disparities.
* **Niche Market Indication:** The highly uneven spread suggests the data likely represents a specific vehicle type or program rather      than general vehicle ownership.

4. **Total Vehicles sold by year**
   ![Total Vehicles sold by Year](https://github.com/user-attachments/assets/fafe2ccc-5c9c-4698-a26a-70a43ca504b7)

* **Steady Growth (2011–2018):** Sales increased from **786 in 2011 to 12,596 in 2018**, reflecting growing consumer interest and         market adoption.
* **Temporary Decline in 2019:** A drop to 9,263 vehicles suggests possible market saturation or external economic pressures.
* **Record Peak in 2023:** Sales surged to an all-time high of **30,366 vehicles**, possibly driven by new model launches or favorable     policies.
* **Significant Drop in 2024:** A sharp fall to 305 vehicles likely points to incomplete data or a major market disruption.
* **Overall Trend:** Despite short-term fluctuations, the long-term trend shows strong market expansion from 2011 to 2023.

5. **City wise Total PHEV**
   ![City wise Total PHEV](https://github.com/user-attachments/assets/41af4401-e806-4b72-916a-0e297816fbe4)

* **Seattle leads** significantly with **4,330 PHEVs**, far surpassing all other cities and indicating it as a central hub for PHEV        adoption.
* **Vancouver (1,091) and Bellevue (810)** follow distantly, suggesting more moderate adoption in these cities.
* Mid-tier adoption is seen in **Olympia, Tacoma, Kirkland, Redmond**, and others, with counts ranging between **400–700 vehicles**.
* **Color Gradient Usage:** Darker green shades effectively highlight cities with higher PHEV concentrations, enhancing visual clarity.
* **Adoption Pattern:** The steep drop after Seattle suggests PHEV adoption is highly localized, likely influenced by city                  infrastructure, environmental incentives, or socio-economic factors.

## Conclusion
* This analysis provides a comprehensive overview of vehicle adoption trends with a focus on clean energy and hybrid vehicles. The data    reveals strong regional disparities, significant gaps in eligibility information, and fluctuating sales trends over time.
* While cities like Seattle and states like Washington are leading the transition toward cleaner vehicles, broader adoption will           require better data practices, targeted infrastructure investments, and policy-driven incentives. These findings can guide               stakeholders in optimizing strategies for clean vehicle adoption and ensuring more data-driven decisions moving forward.










