# Endterm project for Big Data in Law Enforcement
Group: CS-2121  
Authors: Arman Alpar, Raiskanov Rasul

This project focuses on analyzing shooting incidents in New York City using a real dataset and processing it with Pandas, Matplotlib, Folium, and Apache Spark. It explores various aspects of the data such as demographics, geospatial mapping, and temporal trends.

---

## Dataset

The dataset used is:  
**nypd-shooting-incident-data-historic-1.csv**  
It contains historical records of shooting incidents in NYC, including information such as date, time, borough, victim and perpetrator demographics, and geolocation.

---

## Technologies Used

- Python
- Pandas
- Matplotlib
- Folium
- NumPy
- PySpark
- Jupyter Notebook

---

## Project Features

### 1. Data Loading and Overview

- Load CSV using `pandas.read_csv()`
- Initial exploration: `df.head()`, `df.info()`, `df.describe()`

### 2. Data Preprocessing

- Convert `OCCUR_DATE` and `OCCUR_TIME` into datetime
- Create a combined datetime index for resampling
- Resample incidents by month to identify trends

### 3. Time Series Analysis

- Visualize monthly shooting incidents using `matplotlib`

### 4. Geospatial Visualization

- Use `folium` to plot markers for each incident on an interactive NYC map

### 5. Demographic Analysis

- Breakdown of age, sex, and race for both perpetrators and victims

### 6. Apache Spark Integration

- Load the same dataset using PySpark
- SQL queries for:
  - Total incidents
  - Incidents per borough
  - Average location
  - Most violent day

- Plot daily incident trends using Spark and visualize with `matplotlib`

---

## Project Structure

- `End.ipynb` — Main notebook with all data analysis and visualizations
- `nypd-shooting-incident-data-historic-1.csv` — Dataset
- `README.md` — This documentation

---

## How to Run

1. Install the required Python libraries:
   ```bash
   pip install pandas matplotlib folium numpy pyspark
   ```

2. Run the Jupyter notebook:
   ```bash
   jupyter notebook End.ipynb
   ```

3. For Spark processing, ensure you have Java and Spark properly installed.

---

## Highlights

- Most incidents occurred in **Brooklyn**.
- The day with the **maximum incidents** recorded was **July 20, 2013**, with **19** incidents.
- Victims and perpetrators are predominantly male and of Black ethnicity.
- Interactive map shows precise locations of incidents across NYC.

---

## License

This project is for academic use only.
