# **Agricultural Insights Dashboard using ELK Stack**

## **Objective**
The primary objective of this project is to build an **interactive agricultural dashboard** using the **ELK Stack (Elasticsearch, Logstash, and Kibana)**. The goal is to analyze and visualize key factors influencing crop yield, such as rainfall, temperature, soil type, and fertilizer use, enabling better decision-making for stakeholders in the agriculture industry.

---

## **Source and Scope of Dataset**
The dataset used for this analysis was collected **three months ago** and includes **1,000,000 samples** from various regions. It captures critical agricultural metrics aimed at optimizing farming practices, improving yield efficiency, and understanding regional variances.

---

## **Process Workflow**

1. **Data Collection**:  
   - Gather agricultural data covering key metrics such as rainfall, temperature, soil type, and yield.  

2. **Data Transformation and Ingestion**:  
   - **Logstash** pipelines process and ingest the dataset into **Elasticsearch** for efficient querying.

3. **Visualization in Kibana**:  
   - Create insightful visualizations in **Kibana** to interpret data trends and outcomes.  

4. **Dashboard Development**:  
   - Combine visualizations into an interactive dashboard for stakeholders to derive actionable insights.

---

## **Dataset Attributes**

| Attribute           | Description                                                                                 |
|---------------------|---------------------------------------------------------------------------------------------|
| **Region**          | Geographical area: North, East, South, West.                                               |
| **Soil_Type**       | Type of soil: Clay, Sandy, Loam, Silt, Peaty, Chalky.                                      |
| **Rainfall_mm**     | Rainfall received (in millimeters) during crop growth.                                     |
| **Temperature_Celsius** | Average temperature (°C) during the growing season.                                   |
| **Fertilizer_Used** | Whether fertilizers were applied: TRUE/FALSE.                                              |
| **Days_to_Harvest** | Time taken to harvest crops (days).                                                        |
| **Yield_tons_per_hectare** | Total yield per hectare (tons).                                                     |
| **Weather_Condition** | Growing weather: Sunny, Rainy, Cloudy.                                                   |

---

## **Technologies Used**
- **Elasticsearch**: Data storage and querying.  
- **Logstash**: Data processing and ingestion.  
- **Kibana**: Data visualization and dashboard creation.  
- **Python**: Data preparation and pipeline scripting (if needed).  

---
## Dashboard Photo

![ELK](https://github.com/user-attachments/assets/15991fd9-ba3d-4bfc-b4fc-175c9957a629)


---
## Video

https://github.com/user-attachments/assets/ce3caec1-a0ab-4182-8480-07ff0be9c5fa

---
## **Detailed Insights from Dashboard**

### 1. **Overall Insights**
- **Average Days to Harvest**: **102 days**.  
   *Insight*: On average, most crops take approximately 3.5 months to mature. Planning harvest cycles is crucial for labor allocation and logistics.  

- **Average Yield per Hectare**: **4.614 tons/hectare**.  
   *Insight*: This metric serves as a baseline to assess yield performance across regions, soil types, and weather conditions.

- **Average Rainfall**: **520.886 mm**.  
   *Insight*: Indicates that most regions received moderate rainfall suitable for crop growth.

- **Median Temperature**: **27.724°C**.  
   *Insight*: Temperature is within the optimal range for many crops, though regional variations exist.

---

### 2. **Region-Specific Insights**
- **Rainfall by Region**:  
   - **North** received the **highest median rainfall** (~700 mm).  
   - Other regions (West, South, East) received approximately **400-500 mm**.  
   *Managerial Insight*:  
   Regions receiving higher rainfall can focus on water-dependent crops (e.g., rice). Excessive rainfall management strategies like drainage systems are essential.  

- **Temperature Distribution**:  
   - **East** had the **highest median temperature** (~35°C).  
   - **South** had the lowest (~27°C).  
   *Managerial Insight*:  
   High temperatures in the East may require heat-resistant crops or irrigation scheduling to avoid water stress.

- **Days to Harvest by Region**:  
   - **East** recorded the highest average (~120 days).  
   - Other regions are relatively consistent (~100-110 days).  
   *Insight*: Longer harvest times in the East may affect resource allocation and productivity planning.

---

### 3. **Impact of Fertilizer Usage on Yield**
- Yield is significantly higher where **fertilizers were used**:  
   - **TRUE**: ~8 tons/hectare.  
   - **FALSE**: ~4 tons/hectare.  
   *Managerial Insight*:  
   Fertilizer application nearly **doubles the yield**, highlighting its critical role in enhancing productivity. Farmers and stakeholders should prioritize proper fertilizer application techniques.

---

### 4. **Yield by Soil Type**
- **Peaty Soil** had the **highest yield** (~155 tons/hectare).  
- Other soil types such as **Clay (112 tons)** and **Silt (108 tons)** also performed well.  
- **Sandy and Chalky soils** had the **lowest yields** (~95 tons).  
   *Managerial Insight*:  
   - Peaty and Clay soils are more fertile and suitable for high-yield crops.  
   - Strategies such as soil conditioning can improve yields on Sandy and Chalky soils.

---

### 5. **Rainfall Trends Over Time**
- Rainfall fluctuates significantly over time, peaking periodically.  
   *Insight*: Monitoring rainfall patterns can help farmers prepare for irrigation or drainage to maintain crop health during unpredictable weather.

- **Rainfall Trends by Region**:  
   - North experienced a **steady decline**, while South and West saw gradual increases.  
   *Managerial Insight*: Understanding regional rainfall trends can optimize water management strategies for specific areas.

---

### 6. **Yield Trends by Weather Conditions**
- **Cloudy and Rainy weather** led to higher yields compared to **Sunny weather**.  
   *Insight*: Rainfall and moderate sunlight promote better yields, but excessive sunlight without irrigation may reduce productivity.  

---

### 7. **Temperature Trends Over Regions**
- Temperature fluctuated across regions, with East experiencing the **highest peaks**.  
   *Managerial Insight*: Temperature variability requires adaptive practices such as crop rotation or selection of heat-tolerant crops.

---

## **Managerial Insights**

1. **Focus on Fertilizer Use**:  
   - Fertilizer application can **double the yield**. Training farmers on optimal fertilizer use will significantly boost production.

2. **Optimize Regional Practices**:  
   - **North**: Utilize rainfall efficiently for water-dependent crops.  
   - **East**: Implement irrigation to counter high temperatures and water loss.  
   - **South and West**: Moderate rainfall and temperature are ideal for diverse crops.

3. **Soil-Specific Strategies**:  
   - Prioritize high-yield soils like **Peaty and Clay** for intensive farming.  
   - Invest in soil enhancement techniques for **Sandy and Chalky soils**.

4. **Monitor Weather Trends**:  
   - Rainy and Cloudy weather improve yields. Predictive weather modeling can assist in planning irrigation schedules and crop selection.

5. **Harvest Planning**:  
   - East region requires additional focus due to longer harvest durations, impacting labor costs and logistics.

---

## **Learnings from the Project**

1. **ELK Stack Integration**:  
   - Leveraging ELK Stack allowed seamless ingestion, transformation, and visualization of a large-scale agricultural dataset.

2. **Data-Driven Insights**:  
   - Using interactive dashboards enabled granular analysis of regional, soil, and weather-specific factors influencing crop yields.

3. **Decision-Making**:  
   - Data visualizations provided clear insights for stakeholders to make informed decisions about irrigation, fertilizer application, and crop planning.

4. **Scalability**:  
   - The ELK Stack's scalability ensures the platform can handle larger datasets in real-time for future analysis.

5. **Impact of Data Visualization**:  
   - Visualizing complex agricultural data in charts and graphs made it easier for stakeholders to identify actionable insights.

---
