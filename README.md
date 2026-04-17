# Weather & Vacation API Analysis

## Overview
A two-part Python project using the OpenWeatherMap and Geoapify APIs to analyze 
global weather patterns relative to latitude, then use those findings to identify 
ideal vacation destinations and locate nearby hotels.

---

## Part 1 — WeatherPy

Analyzed weather data from 500+ randomly selected cities worldwide to answer:
**"What is the weather like as we approach the equator?"**

### Scatter Plots
- Latitude vs. Temperature
- Latitude vs. Humidity
- Latitude vs. Cloudiness
- Latitude vs. Wind Speed

### Linear Regression Analysis
Computed linear regression for each weather variable, split by hemisphere:
- Northern Hemisphere vs. Southern Hemisphere comparisons for all four variables
- R² values and regression formulas included on each plot

---

## Part 2 — VacationPy

Used weather data from Part 1 to identify ideal vacation cities and find hotels.

- Mapped all cities with point size scaled by humidity
- Filtered cities to ideal weather conditions:
  - Max temperature between 21–27°C
  - Wind speed under 4.5 m/s
  - Zero cloudiness
- Used Geoapify API to find the nearest hotel within 10,000 meters of each city
- Displayed hotels on an interactive map with city, country, and hotel name in 
  hover tooltips

---

## Tech Stack
- Python (Pandas, Matplotlib, Requests, citipy, geoViews)
- OpenWeatherMap API
- Geoapify API
- Jupyter Notebook

---

## Repository Contents
| File | Description |
|------|-------------|
| `WeatherPy.ipynb` | Weather analysis and regression notebook |
| `VacationPy.ipynb` | Vacation planning and hotel mapping notebook |
| `output_data/` | Generated plots and city data CSV |
