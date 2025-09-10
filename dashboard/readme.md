# 📊 Dashboard 

This folder contains the Power BI dashboard visuals created for the Cyclistic Bike-Share Capstone Project.  
The dashboard highlights **rider behavior differences** between casual riders and members, and supports strategies to increase memberships.

---

## 🧹 Data Cleaning & Preprocessing (Power Query)

Before building the visuals, I cleaned and transformed the raw dataset in **Power Query**:

1. **Removed null values** in start time, end time, and rider type columns.  
2. **Removed duplicate rows** to avoid double-counting trips.  
3. **Added calculated columns**:
   - `ride_length` = end time – start time  
   - `day_of_week` = extracted weekday name from start date  
   - `month` = extracted month from start date  
4. **Formatted columns** (date/time to proper data types).  
5. **Filtered out invalid rides** (e.g., ride length ≤ 0).  
<img width="871" height="484" alt="google data analyst rider dashboard" src="https://github.com/user-attachments/assets/6d351e52-dee1-4104-baa5-77691f9b091f" />

---

## 📊 Visualizations & Purpose

### 1. KPI Cards
- **Visuals:** Total rides, Member count, Casual count, Average ride duration.  
- **Why:** Provides a quick snapshot of overall usage and key metrics.  

---

### 2. Average Ride Duration (Casual vs. Member)
- **Visual:** Clustered column chart.  
- **Why:** Shows that casual riders take ~2x longer rides, while members ride shorter trips more frequently.  

---

### 3. Ride Trends by Day of Week
- **Visual:** Clustered column chart (Mon–Sun).  
- **Why:** Casual riders peak on weekends → leisure behavior.  
  Members ride mostly on weekdays → commuting behavior.  

---

### 4. Ride Trends by Month
- **Visual:** Line chart.  
- **Why:** Casual rides drop sharply in winter, while members remain steady year-round.  

---

### 5. Bike Type Usage
- **Visual:** Stacked bar chart (Classic, Docked, Electric bikes).  
- **Why:** Members prefer **classic bikes** for commuting, casuals prefer **electric bikes** for leisure.  

---

## 🎯 Dashboard Key Takeaway
- Casual riders = long, seasonal, weekend rides (leisure/tourism).  
- Members = short, frequent, weekday rides (commuting).  
- By targeting casual riders with flexible memberships, seasonal discounts, and electric bike offers, Cyclistic can drive membership growth and sustain revenue.
