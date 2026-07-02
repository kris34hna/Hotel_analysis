# Hotel Booking Project

Analyzing hotel booking data to uncover the key factors driving cancellation rates and providing actionable business recommendations to help City Hotel and Resort Hotel reduce cancellations and improve revenue.

---

## Brief Summary

An exploratory data analysis (EDA) project on 1,19,390 hotel bookings — involving data cleaning, feature engineering, and visualization using Python — to answer: "What are the variables that affect hotel reservation cancellations and how can hotels make better pricing and promotional decisions?"

---

## Overview

In recent years, City Hotel and Resort Hotel have seen high cancellation rates. Each hotel is now dealing with a number of issues as a result, including fewer revenues and less than ideal hotel room use. Consequently, lowering cancellation rates is both hotels' primary goal in order to increase their efficiency in generating revenue. This project analyses booking cancellations as well as other factors that have no bearing on their business and yearly revenue generation.

---

##Problem Statement

In recent years, City Hotel and Resort Hotel have seen high cancellation rates. Each hotel is now dealing with a number of issues as a result, including fewer revenues and less than ideal hotel room use. Consequently, lowering cancellation rates is both hotels' primary goal in order to increase their efficiency in generating revenue, and for us to offer thorough business advice to address this problem.

####Research Questions:

Question1What are the variables that affect hotel reservation cancellations?2How can we make hotel reservations cancellations better?3How will hotels be assisted in making pricing and promotional decisions?

Hypotheses:

Hypothesis1More cancellations occur when prices are higher2When there is a longer waiting list, customers tend to cancel more frequently3The majority of clients are coming from offline travel agents to make their reservations

---

##Dataset

| Column | Description |
|--------|-------------|
| hotel | Hotel type — City Hotel or Resort Hotel |
| is_canceled | Target variable — 1 = Canceled, 0 = Not Canceled |
| lead_time | Days between booking and arrival |
| arrival_date_month | Month of arrival |
| stays_in_weekend_nights | Number of weekend nights booked |
| stays_in_week_nights | Number of weekday nights booked |
| adults | Number of adults |
| children | Number of children |
| babies | Number of babies |
| meal | Meal plan selected |
| country | Country of origin of guest |
| market_segment | Market segment — Online TA, Offline TA, Direct, Corporate, etc. |
| distribution_channel | Booking distribution channel |
| is_repeated_guest | Whether guest is a repeat visitor |
| previous_cancellations | Number of previous cancellations |
| adr | Average Daily Rate (room price per night) |
| days_in_waiting_list | Days on waiting list before confirmation |
| customer_type | Transient, Contract, Group, Transient-Party |
| deposit_type | No Deposit, Non Refund, Refundable |
| reservation_status_date | Date of last reservation status update|

---

## Tools & Technologies

| Tool | Purpose |
|------|---------|
| Python (Jupyter Notebook) | Data cleaning, EDA & visualization |
| Pandas / NumPy | Data manipulation & feature engineering |
| Matplotlib / Seaborn | Visualizations (pie charts, bar charts, countplots, line charts) |
| Squarify | Treemap chart for market segment analysis |

---

## Methods

| Step | Description |
|------|-------------|
| Initial Inspection | Checked shape (1,19,390 × 32), data types, null value %, and duplicates |
| Data Cleaning | Converted reservation_status_date to datetime, dropped 4 irrelevant/high-null columns (company, reservation_status, arrival_date_year, agent), dropped remaining null rows|
| Outlier Removal | Removed bookings with zero total guests (adults + children + babies = 0) and invalid ADR values (negative or > 5000) |
| Feature Engineering | Extracted month from reservation_status_date for monthly trend analysis |
| Univariate Analysis | Overall cancellation pie chart · Hotel-wise cancellation pie charts · Market segment treemap (all bookings vs cancelled) |
| Bivariate Analysis | Reservation status per month (countplot) · City Hotel monthly cancellations · ADR per month for City Hotel cancelled bookings |
| Geographical Analysis | Top 10 countries with highest cancellations (pie chart) |
| Price vs Cancellation | ADR trend comparison — cancelled vs not cancelled bookings (2016–2017 line chart) |

---

## Key Insights

1. Price drives cancellations — cancelled bookings consistently show higher Average Daily Rate (ADR) than non-cancelled ones, confirming Hypothesis 1.
2. City Hotel has a higher cancellation ratio than Resort Hotel — city hotels need more aggressive pricing and discount strategies.
3. January has the highest cancellation rate across months — ideal time for targeted marketing campaigns to recover revenue.
4. Portugal (PRT) dominates cancellations — the top country by far in the top 10 cancelled bookings pie chart.
5. Online Travel Agents (OTA) are the largest market segment for both total and cancelled bookings — reducing OTA dependency could lower cancellation risk.
6. Longer waiting lists are associated with higher cancellation likelihood — customers lose interest or find alternatives.
7. ADR trend confirms seasonality — room prices peak in summer months and cancellations follow the same pattern.
8. Resort Hotels see higher ADR spikes on weekends and holidays compared to City Hotels — pricing strategy should differ by hotel type.

---

## Results & Conclusion

The analysis confirms that price (ADR) is the strongest driver of cancellations — when room rates are high, cancellations spike, especially in City Hotels. Portugal is the top source of cancellations geographically, and Online Travel Agents contribute the most to both total and cancelled bookings. January is the most vulnerable month revenue-wise. These findings validate all 3 hypotheses and provide a clear direction for hotels to redesign their pricing, discount, and marketing strategies to recover lost revenue.

---

### Suggestions

1. Lower prices strategically — cancellation rates rise with price; hotels should work on location-based pricing and offer discounts to reduce cancellations.
2. Weekend & holiday discounts for City Hotel — since City Hotel has a higher cancellation ratio, reasonable weekend/holiday discounts can improve retention.
3. January marketing campaigns — January has the highest cancellation month; hotels should launch targeted campaigns with competitive pricing to boost revenue.
4. Improve quality in Portugal — since Portugal leads cancellations, improving hotel quality and services there can significantly reduce the cancellation rate,

---

## Author & Contact

| Field | Info |
|-------|------|
| Name |KRISHNA |
| LinkedIn | https://www.linkedin.com/in/krishna-krishna-26a106231/ |
| GitHub | https://github.com/ |


⭐ If you found this project helpful, consider giving it a star!
