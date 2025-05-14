
```markdown
# HVAC Sensor Data Analysis  
**Sanjai Kumar G
**  
**II Year – Mechanical Engineering**  
**Course:** Data Analysis in Mechanical Engineering  
**College:** ARM College of Engineering & Technology  

---

## Project Introduction

This project focuses on analyzing data collected from an HVAC system (Heating, Ventilation, and Air Conditioning). The goal is to understand how different indoor conditions — like temperature, humidity, air flow, and occupancy — affect energy usage and overall system behavior.

As a mechanical engineering student, this project helped me connect real-world environmental control systems with data analysis. By studying sensor readings over time, we can gain useful insights for improving both comfort and energy efficiency in buildings.

---

## About the Dataset

The dataset contains time-stamped readings from various HVAC-related sensors. Below is a quick overview of the main features included:

| Feature Name              | What It Measures                                 |
|--------------------------|--------------------------------------------------|
| Date_Logged              | Time when the data was recorded                  |
| Temperature (C)          | Indoor air temperature (Celsius)                 |
| Humidity (%)             | Relative humidity in percentage                  |
| Air_Flow (CFM)           | Airflow rate in Cubic Feet per Minute            |
| CO2_Level (ppm)          | Indoor CO₂ concentration in parts per million    |
| Occupancy                | Number of people present in the space            |
| Energy_Consumption (kWh) | Total energy used by the HVAC system (kWh)       |

---

## Data Preprocessing Steps

To prepare the data for analysis, the following steps were performed:

1. **Importing the Dataset**  
   Loaded the dataset using pandas and checked the structure of the data.

2. **Datetime Formatting**  
   Converted the `Date_Logged` column to datetime format for easier time-based grouping.

3. **Handling Missing Data**  
   Missing values in columns like `CO2_Level (ppm)` and `Air_Flow (CFM)` were filled with their mean values.

4. **Creating New Features**  
   To support deeper analysis, two new columns were added:
   - `Hour`: Extracted from the timestamp.
   - `DayOfWeek`: Represents which day of the week the data point falls on.

---

## Exploratory Data Analysis (EDA)

During the EDA phase, several visual tools were used to explore the data and find patterns:

### 1. Time-Based Patterns  
- Energy consumption shows a repeating pattern, especially during typical working hours.
- CO₂ levels and indoor temperature also vary based on occupancy levels.

### 2. Correlation Study  
- There is a clear relationship between occupancy and CO₂ levels.
- Energy usage tends to rise with both air flow and temperature.

### 3. Feature Distributions  
- Histograms and boxplots showed that some values, especially in airflow and energy usage, may have outliers or be slightly skewed.

---

## Key Observations

- **CO₂ levels rise when more people are present**, confirming that occupancy affects indoor air quality.
- **Air flow increases with occupancy**, suggesting that the HVAC system adjusts automatically.
- **Peak energy usage** occurs between 9 AM and 6 PM, which is aligned with regular work hours.
- **Temperature and humidity remain fairly stable**, showing the HVAC system works efficiently most of the time.

---

## Future Improvements

- Apply outlier detection techniques to clean the data further (e.g., using IQR).
- Build a predictive model to forecast energy consumption or detect unusual patterns in HVAC behavior.
- Explore how external weather data might influence HVAC system performance (as an extension).

---

## Tools and Technologies Used

- **Python** – Core programming language  
- **Pandas, NumPy** – For working with data and arrays  
- **Matplotlib, Plotly** – For creating clear and informative visualizations  
- **Jupyter Notebook** – Used to run code and document the steps in an organized way  

---

## Conclusion

Through this project, I learned how sensor data from mechanical systems can be analyzed using data science techniques. This kind of analysis helps in making smart decisions for energy savings and comfort in buildings. It was a valuable learning experience, especially as a beginner exploring the role of data in mechanical engineering systems.
```
