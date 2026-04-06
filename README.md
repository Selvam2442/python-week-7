# COVID-19 Data Analysis and Interactive Dashboard

## Overview
This project performs an exploratory data analysis (EDA) and visualization of a global COVID-19 dataset. It features data cleaning, static statistical charts to uncover global trends, correlation analyses between different case outcomes, and an interactive web dashboard built with Dash to explore the spread of the virus over time by specific countries.

## Features
* **Data Preprocessing:** Cleans the raw dataset by handling missing values, standardizing datetime formats, and removing duplicate records.
* **Time Series Analysis:** Visualizes cumulative and daily new confirmed COVID-19 cases globally.
* **Country-Level Insights:** Identifies and plots the top 10 most affected countries based on total confirmed cases, deaths, and recoveries.
* **Interactive Dashboard:** Features a Jupyter Dash application with a country dropdown and date-range picker to dynamically filter and view cumulative cases for specific regions.
* **Correlation Analysis:** Utilizes Plotly scatter plots and a Seaborn heatmap to examine the relationships between confirmed, active, recovered cases, and deaths.
* **Global Distribution:** Displays the overall ratio of active, recovered, and fatal cases using interactive pie charts.

## Technologies & Libraries Used
* **Python 3**
* **Data Manipulation:** `pandas`, `numpy`
* **Static Visualization:** `matplotlib.pyplot`, `seaborn`
* **Interactive Visualization:** `plotly.express`
* **Web Dashboard:** `jupyter_dash`, `dash` (including `dash_core_components` and `dash_html_components`)

## Dataset
The project utilizes a dataset named `covid_19_clean_complete.csv`. It contains the following key data points:
* `Country/Region` and `Province/State`
* `Lat` and `Long` (Geographical coordinates)
* `Date` of the record
* `Confirmed`, `Deaths`, `Recovered`, and `Active` case counts
* `WHO Region`

## Setup and Installation

1. Download the Jupyter Notebook (`project_7.ipynb`) and the required dataset.
2. Update the file path in the notebook's `pd.read_csv()` function to point to your local or cloud directory where the dataset is stored.
3. Install the required Python libraries. You can do this by running the following command in your terminal or command prompt:

```bash
pip install pandas numpy matplotlib seaborn plotly dash jupyter-dash
