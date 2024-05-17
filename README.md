# EDA-Hotel-booking-analysis


## Project Overview

This project involves analyzing hotel bookings data to uncover insights into booking patterns, distribution channels, and guest demographics. The analysis includes various visualizations and statistical analyses to provide a comprehensive understanding of the data.

## Dataset

The dataset used in this analysis contains information on hotel bookings, including details about arrival dates, length of stay, number of guests, booking sources, and pricing. Key columns include:
- `hotel`: Type of hotel (Resort Hotel or City Hotel)
- `is_canceled`: Whether the booking was canceled
- `lead_time`: Number of days between booking and arrival
- `arrival_date_month`: Month of arrival
- `adr`: Average Daily Rate (price per day of stay)
- `distribution_channel`: Booking distribution channel (e.g., Direct, TA/TO)
- `adults`, `children`, `babies`: Number of adults, children, and babies
- arrival_date_year: Year of arrival date.
- arrival_date_week_number: Week number of the year for the arrival date.
- arrival_date_day_of_month: Day of the month for the arrival date.
- stays_in_weekend_nights: Number of weekend nights (Saturday or Sunday) the guest stayed or booked to stay at the hotel.
- stays_in_week_nights: Number of week nights (Monday to Friday) the guest stayed or booked to stay at the hotel.


## Analysis
### Grouping by Distribution Channel and Hotel Type
- **Objective**: Calculate the average ADR for each distribution channel and hotel type.
- **Method**: Group the data by `distribution_channel` and `hotel`, then calculate the mean of `adr`.

### Monthly Bookings Analysis
- **Objective**: Count the number of bookings for each month.
- **Method**: Group the data by `arrival_date_month` and count the number of records.

## Visualizations
- **Heatmap**: Visualizes the correlation between different numeric columns in the dataset.
- **Bar Plot**: Shows the number of bookings per month.
- **Grouped Bar Plot**: Compares the average ADR across different distribution channels and hotel types.
- **Pie chart**: To show the distribution of percentage in cancelled and no cancelled bookings.
- **Pair plot** To show relationship in single vables with others.


  ### Example Plots
```python
# Code snippets for generating plots
import matplotlib.pyplot as plt
import seaborn as sns
import pandas as pd
import numpy as np


Insights
- Based on the analysis and visualizations, several insights were derived:
- Distribution Channel Impact: Certain distribution channels tend to have higher ADRs, indicating a potential focus area for maximizing revenue.
- Monthly Trends: Booking volumes vary significantly by month, with peak and off-peak seasons identified.
- Hotel Type Preferences: Differences in ADR between resort and city hotels suggest varying pricing strategies or customer demographics.
