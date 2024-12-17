# Hotel_Booking_Cancellation_Analysis

This repository contains a comprehensive analysis of hotel booking data, with a focus on understanding the factors contributing to booking cancellations. The dataset includes information from two hotels: a city hotel and a resort hotel. The goal of this analysis is to provide insights that can help reduce cancellation rates and optimize hotel revenue. 

<br>

## About Dataset

Dataset was taken from kaggle, it contains 119390 observations for a City Hotel and a Resort Hotel. Each observation represents a hotel booking between the 1st of July 2015 and 31st of August 2017, including booking that effectively arrived and booking that were canceled. Since this is hotel real data, all data elements pertaining hotel or costumer identification were deleted. Four Columns, 'name', 'email', 'phone number' and 'credit_card' have been artificially created and hence, they were also deleted. Therefore, updated dataset includes 119390 rows and 36 columns.

The link for the dataset from kaggle can be found [Hotel_Booking _Dataset](https://www.kaggle.com/datasets/mojtaba142/hotel-booking)

<br>

## Business Problem

City Hotel and Resort Hotel are experiencing high cancellation rates, which impact their revenue and room occupancy. The main objective of this analysis is to identify the factors that lead to cancellations and provide actionable insights to reduce cancellations and improve revenue generation.

<br>

## Research Questions

1. What are the variables that affect hotel reservation cancellations?
2. How can we reduce the number of cancellations?
3. How can hotels use this information to make better pricing and promotional decisions?

<br>

## Hypotheses

- Higher booking prices lead to more cancellations.
- Longer waiting lists contribute to higher cancellation rates.
- Guests from certain market segments, such as online travel agencies, are more likely to cancel.

<br>

## Analysis and Findings

In the Jupyter notebook (`hotel_booking_da.ipynb`), several steps were taken to clean, analyze, and visualize the dataset:

### 1. **Data Cleaning**
   - Missing values were handled, particularly in columns like `children`, `country`, and `agent`.
   - Outliers were identified and managed, especially for columns like `lead_time` and `adr`. (adr is Average daily rate for the booking)

### 2. **Exploratory Data Analysis (EDA)**
   - **Cancellation Rates**: The percentage of canceled and non-canceled bookings was analyzed using bar plots, showing that about 37% of the bookings were canceled, significantly impacting hotel revenue.
   - **Monthly Analysis**: A grouped bar graph was created to examine the number of confirmed and canceled bookings by month. August had the highest number of cancellations, while January showed the highest cancellation ratio.
   - **Price vs. Cancellations**: A line plot revealed that cancellations are more likely when the average daily rate (ADR) is higher. This was a key factor contributing to booking cancellations, as customers tend to cancel when prices rise.

### 3. **Key Findings**
   - **Price Sensitivity**: Bookings are more likely to be canceled when prices are higher, especially for resort hotels during weekends and holidays.
   - **Country of Origin**: Guests from Portugal were found to have the highest cancellation rates.
   - **Market Segment**: Most cancellations came from online travel agents (46%), followed by group bookings.

### 4. **Visualization Highlights**
   - **Booking Cancellations by Month**: Visualized the cancellation trends across different months, with peak cancellations in August.
   - **Market Segments**: Explored the distribution of bookings from various segments (e.g., online travel agents, direct bookings).
   - **ADR and Cancellation Trends**: Highlighted that high ADR values correlate with higher cancellation rates, reinforcing the importance of pricing strategies.

### 5. **Suggestions for Reducing Cancellations**
   - **Dynamic Pricing**: Implement dynamic pricing strategies that adjust based on demand to reduce cancellations during peak periods.
   - **Targeted Marketing**: Focus marketing campaigns in January to reduce cancellations and increase bookings during this low period.
   - **Service Improvement**: Consider improving services, especially for markets with high cancellation rates like Portugal, to encourage customer retention.

<br>

## Files in the Repository

- **`hotel_bookings2.csv`**: The dataset used for the analysis.
- **`hotel_booking_da.ipynb`**: The Jupyter Notebook containing the data analysis code.
- **`hotel-report.pdf`**: A detailed report on the analysis and findings.

<br>

## Conclusion

This project provides a detailed analysis of hotel booking data, with actionable insights to reduce cancellations and improve hotel revenue. By adjusting pricing strategies and focusing on specific market segments, hotels can minimize the impact of cancellations on their business.
