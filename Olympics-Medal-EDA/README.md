# Olympics_Medal_EDA

---

## Olympic Data Analysis with Streamlit

This repository contains a **Streamlit** web application that performs **Olympic Games data analysis**. The project uses historical data of athletes and their achievements across multiple sports and countries. The analysis includes:
- Visualizations of the number of medals won by countries in different sports.
- Country-wise participation across all sports.
- Medal-wise breakdowns for various sports.


### Features

- **Sport-wise Analysis of Countries**: The application allows users to input a country and a sport and visualize the number of gold, silver, and bronze medals won by that country in the specified sport.
- **Country Participation**: Analyze which countries participate in specific sports and how often they compete.
- **Historical Data**: Insights are based on the `athlete_events.csv` dataset, which contains data from multiple Olympic events.
  
Due to the large size of the dataset, deployment on **Streamlit**'s cloud platform faced issues. A working video of the application is attached for reference.


### Files

### 1. `app.py`
This is the main script that runs the **Streamlit** application. The script includes the following functionalities:
- Filters data based on the input country and sport.
- Visualizes the number of medals won by the selected country in the selected sport using bar charts.
- Displays country participation in different sports over time.
  
### 2. `helpers.py`
Contains helper functions that process and clean the dataset:
- Functions to group and filter the data by country and sport.
- Helper functions to handle the rendering of visualizations in the `app.py` script.

### 3. `athlete_events.csv`
This dataset contains historical data about Olympic athletes, including their names, countries, sports, events, medals won, and other relevant details.

### 4. `noc_regions.csv`
Contains information about the National Olympic Committees (NOCs) and their corresponding regions.

### 5. `notebook.ipnb`
This jupyter file contains analyzing the data and before-hand running of all the functions and manipulations


## Data Sources

- **athlete_events.csv**: Contains information on athletes from all Olympic Games, including their medals.
- **noc_regions.csv**: Provides the mapping between the National Olympic Committees (NOCs) and their corresponding regions.


## Pdf Demo

Since the dataset is large and the application could not be deployed on the Streamlit cloud platform, a **working pdf demo** is attached to this repository. It showcases how the app works with the given data and analysis.


## Challenges

### Data Size
The main challenge faced during the deployment was the **large size of the dataset** (`athlete_events.csv` and `noc_regions.csv`), which exceeded the limits for deployment on **Streamlit Cloud**. For local use, however, the application works perfectly.


## Future Improvements

- **Data Sampling**: In future iterations, sampling techniques could be used to reduce the dataset size for easier deployment.
- **Cloud Storage**: Using a cloud-based data storage solution, such as Google BigQuery or AWS, can help handle large datasets more effectively in the cloud.
- **Advanced Visualizations**: The app can be extended with more detailed visualizations like time-series analysis of medal trends over the years.
