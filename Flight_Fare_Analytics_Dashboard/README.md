# ✈️ Flight Fare Analytics Dashboard (Power BI)

## 📌 Project Overview
This project presents an interactive **Flight Fare Analytics Dashboard** built using **Power BI**, focused on analyzing airline ticket pricing patterns across airlines, routes, travel classes, booking windows, and time-of-day factors.

The dashboard emphasizes **robust price analysis** by using statistically appropriate measures to represent typical flight fares.

---

## 📊 Dataset Summary
- **Total Flight Records:** 300,153  
- **Unique Flights:** 1,561  
- **Operating Airlines:** 6  
- **Median Ticket Fare:** ₹7,425  
- **Average Flight Duration:** 12.22 hours  

---

## 📈 Metric Selection & Statistical Justification

### Why Median Price is Used
All price-related visuals in this dashboard use **Median Ticket Fare** instead of Average (Mean).

#### Skewness Analysis
Using pandas, skewness of ticket prices was calculated:

- **Skewness of Price:** **1.06**

#### Interpretation
- A skewness value greater than **+1** indicates a **right-skewed distribution**
- This confirms the presence of **extreme high-priced tickets** (e.g., business class, last-minute bookings)
- In such distributions, the **mean gets inflated**, while the **median remains stable**

#### Conclusion
**Median price is a statistically robust measure** for this dataset and provides a realistic representation of what a typical passenger pays.  
This ensures **fair and reliable comparison** across airlines, routes, travel classes, and time windows.

---

## 🔍 Key Insights

### 🛫 Airline-wise Fare Comparison
- **Highest Median Fare:** Vistara  
- **Lowest Median Fare:** AirAsia  
- **Indigo** operates the highest number of unique flights (~45%)

---

### ⏳ Booking Window vs Ticket Price
- Prices generally increase closer to departure
- **3–7 days before departure** shows high price variability
- Very early and very late bookings can both result in higher fares depending on route and airline

---

### 🕒 Departure & Arrival Time Analysis
- **Late-night and early-morning flights** tend to have lower median fares
- **Afternoon and evening flights** generally show higher prices

---

### 🧳 Travel Class Impact
- **Business Class:** Very high median fares
- **Economy Class:** Stable and affordable pricing  
Travel class is one of the strongest drivers of ticket price variation.

---

### 🌍 Route-based Pricing
- Certain city pairs consistently show higher median fares
- Pricing behavior varies significantly based on source–destination combinations

---

## 🎛️ Dashboard Features
- Interactive slicers for:
  - Airline
  - Travel Class
  - Source City
  - Destination City
  - Departure Time
  - Arrival Time
- Dynamic visuals:
  - KPI cards
  - Bar charts
  - Heatmaps
- Clean layout focused on analytical clarity

---

## 🛠 Tools & Technologies
- **Power BI Desktop**
- **Power Query (Data Cleaning & Transformation)**
- **DAX (Measures & Calculations)**
- **Python (Pandas for EDA & Skewness Analysis)**

---

## 🎯 Use Cases
- Flight price comparison
- Airline pricing behavior analysis
- Travel cost optimization
- Business intelligence portfolio project

---

## 📁 Repository Structure
- Flight_Fare_Analytics_Dashboard.pbix
- Flight_Fare_Analytics_Dashboard.pdf
- Flight_Fare_Analytics_Dataset.xlsx
- README.md
