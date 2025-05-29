# 🏅 Olympics-data-analysis

<p align="center">
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/5c/Olympic_rings_without_rims.svg/320px-Olympic_rings_without_rims.svg.png" alt="Olympics Logo" width="200"/>
</p>


## 📊 Project Overview

This Power BI project provides an in-depth analysis of the Olympic Games data from 1988 to 2016, visualizing athlete performance, country-wise medal achievements, sport-specific trends, and India's participation across seasons and years.

---

## 🧩 Data Source

- **Dataset**: Olympics dataset (from Kaggle or official sources)
- **Time Range**: 1988 to 2016 (Summer and Winter Olympics)
- **Key Tables**:
  - `athlete_events`
  - `noc_regions`

---

## 🛠️ Data Cleaning & Transformations

### `athlete_events` table:
- Filtered data to include only **1988–2016**
- Removed `height` and `weight` columns
- Replaced nulls in `medal` with `"no medal"`
- Added a **custom column**:  
  ```powerquery
  Medal_Flag = if [Medal] <> "no" then 1 else 0
- Removed nulls from age
- Changed column types appropriately

### noc_regions table:
- Renamed region column to country

## 📌 DAX Measures

### Key measures created:
- Total_Countries
- Medal_winning_countries
- India_total_medals
- Distinct_Athletes
- India_Participants
- Total_Medals
- Total_Gold_Medals
- Total_Silver_Medals
- Total_Bronze_Medals
- Total_Events
- Total_Sports
- Medals_by_country
- Medals_by_sport_gender
- Total_Athletes_by_Sport
- Total_Sports_by_Year
- Total_Medals_by_Sport

## 📁 Dashboards Overview

### 1.🧍 Athlete Dashboard
- Total athletes and medal-winning athletes
- Athlete participation by gender and age
- Top 10 athletes by medal count
- Participation trend line over the years
- Medal type distribution by athletes
- Highlight on India (participation and total medals)

### 2. 🌍 Countries Dashboard
- Total countries and medal-winning countries
- Indian participants over time
- World map of total medals by country
- Athletes by gender and country
- Medal distribution by country
- Top 10 countries by total medals

### 3. 🏅 Sports Dashboard
- Total sports/events
- Medals by sport and gender
- Athletes over time by sport
- Sports by season and year
- Medals by sport (bar and treemap)

## 🔍 Insights

- USA leads in total medal count, followed by Russia and Germany.
- Athletics and Swimming are the most participated sports.
- India's participation has steadily increased since the 2000s.
- Gender participation shows a rising trend for female athletes over time.
- Most medals are awarded in summer games, especially in Swimming and Athletics.

## 🧩 Filters & Slicers Used

- Year
- Country
- Season (Summer/Winter)
- Sport

## 📌 Conclusion

This project provides a comprehensive analysis of Olympic data from 1988 to 2016 using Power BI. The dashboards deliver insights into athlete participation, medal distribution, country performance, and sport-specific trends. Further enhancements can continue to improve usability, aesthetics, and storytelling impact.




