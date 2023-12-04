# Investigate Hotel Business using Data Visualization
Explore hospitality data, visualizing customer behavior in hotel reservations and its impact on cancellations for strategic insights.

## Project Overview 📊

**Business Statement 🏨:**
As a member of the Data Scientist team at a hotel company, the main goal of this Mini Project is to provide insight and in-depth understanding of our hotel's business performance. 🚀 Through data exploration, we will analyze customer behavior in booking hotel tickets, look for factors that influence hotel ticket booking cancellations, and identify opportunities to improve our services and profitability. The results of this analysis will be presented using data visualization and data storytelling to help the management team make smarter and more strategic decisions in managing our hotel business.

**Goals 🎯:**
1. Analyze customer behavior in booking hotel tickets, including booking patterns, length of stay, and room preferences.
2. Identify factors that contribute to hotel ticket booking cancellations, such as price, room type, and booking period.
3. Present discovered insights through informative and easy-to-understand data visualizations. 📈
4. Provide recommendations to the hotel management team based on analysis findings to improve service and profitability. 💼
5. Create powerful data stories to help management teams make smarter, data-driven decisions. 📖

**Objective:**
Creating relevant Report and Visualization for The Business hotel Performance from the data that has been collected.

## Tools for The Project

This project leverages several powerful data analysis and visualization libraries to gain insights and create compelling visualizations:

- **Pandas**: is used for data manipulation, analysis, and cleaning. It provides data structures and functions for working with structured data.
  
![image](https://github.com/riyouuyt/Investigate-Hotel-Business-using-Data-Visualization/assets/122600889/5303d66a-c02d-4384-9587-157f41f508e9)

- **NumPy**: is a fundamental library for scientific computing in Python. It's used for numerical operations, including handling arrays and matrices.
  
![image](https://github.com/riyouuyt/Investigate-Hotel-Business-using-Data-Visualization/assets/122600889/cc10b08d-0ea2-4d93-819b-8d1b3a114ea5)

- **Seaborn (sns)**: is a data visualization library based on Matplotlib. It's used to create attractive and informative statistical graphics.
  
![image](https://github.com/riyouuyt/Investigate-Hotel-Business-using-Data-Visualization/assets/122600889/aaf9fb56-b8af-4e28-aaaf-50bc5d838e20)

- **Matplotlib**: is a widely used data visualization library. It's employed to create a wide range of static, animated, and interactive plots and figures.

![image](https://github.com/riyouuyt/Investigate-Hotel-Business-using-Data-Visualization/assets/122600889/77de4ab7-5558-4307-a429-4ab239557797)


## Data Understanding:

Project Data Column Information: 
* `Hotel type`: (Resort Hotel or City Hotel).
* `is_canceled`: Indicates if the order was canceled (1 = Yes, 0 = No).
* `lead_time`: Number of days between booking date and arrival date.
* `arrival_date_year`: The year the customer arrived.
* `arrival_date_month`: The month the customer arrived.
* `arrival_date_week_number`: Week number in the year of arrival.
* `arrival_date_day_of_month`: Arrival day in month.
* `stays_in_weekend_nights`: Number of weekend nights spent by the customer.
* `stays_in_weekdays_nights`: Number of weeknights spent by the customer.
* `adults`: The number of adults in the booking.
* `children`: Number of children in the booking.
* `babies`: Number of babies in the order.
* `meal`: The type of meal ordered.
* `city`: Destination city code.
* `market_segment`: Customer market segment.
* `distribution_channel`: Order distribution channel.
* `is_repeated_guest`: Signs if the customer is a repeat guest (1 = Yes, 0 = No).
* `previous_cancellations`: Number of orders previously canceled by the customer.
* `previous_bookings_not_canceled`: Number of previous bookings that were not canceled by the customer.
* `booking_changes`: Number of changes made to the booking.
* `deposit_type`: Type of deposit paid (No Deposit, Non Refund, or Refundable).
* `agent`: ID of the agent who placed the order.
* `company`: Company ID if the order was made by a company.
* `days_in_waiting_list`: The number of days in the waiting list before the booking is confirmed.
* `customer_type`: Customer type (Transient, Contract, or Group).
* `adr`: Average Daily Rate, average daily rate.
* `required_car_parking_spaces`: Number of parking spaces required by the customer.
* `total_of_special_requests`: Number of special requests submitted by customers.
* `reservation_status`: Reservation status (Canceled, Check-Out, or No-Show).



## Data Preprocessing

In the quest for meaningful insights, our data underwent a meticulous data preprocessing journey. These essential steps were taken to refine the dataset, ensuring its quality and usability:

**1. Removing Duplicate Data**
   - Duplicate records were unearthed and skillfully expunged from the dataset. This meticulous process guarantees that each entry within the dataset is unique, eliminating redundancy and maintaining data integrity.

**2. Correcting Data Types**
   - Data type corrections were meticulously made for select columns, ensuring the data accurately represents the information they contain. This critical step guarantees that calculations and operations on the data are executed flawlessly.

**3. Handling Invalid Data**
   - Forged in the fires of data scrutiny, we addressed invalid or missing data values with precision. In certain columns, missing values were gracefully filled with zero, while 'unknown' values were judiciously assigned in cases where data was elusive.

**4. Dropping Unnecessary Data**
   - With a discerning eye, we pruned the dataset of superfluous columns that contributed little to our analysis or bore no relevance to the project's objectives. This trimming process streamlines the dataset, enhancing focus and efficiency for the analytical journey.

These artful data preprocessing steps were expertly executed to prepare the data for an in-depth analysis, guaranteeing the accuracy and integrity of the insights waiting to be unveiled.


## Monthly Hotel Booking Analysis Based on Hotel Type

![image](https://github.com/riyouuyt/Investigate-Hotel-Business-using-Data-Visualization/assets/122600889/1cdd2930-f9cc-4275-82db-452bb4451d09)

Assumptions:
* The highest values for reservations, cancellations, and bookings in the summer months, particularly from `April` to `August`, could be due to the peak vacation season when more tourists and travelers choose to book hotels.
* The lowest values in `January`, `February`, and `march` may be attributed to the post-holiday and off-peak travel periods, resulting in fewer bookings.
* `September` and `October` have three "Total Years" of data, which might be due to unique events or factors impacting hotel bookings during those months. Further investigation is needed to determine the cause of this data anomaly.

## Impact Analysis of Stay Duration on Hotel Bookings Cancellation Rates

![image](https://github.com/riyouuyt/Investigate-Hotel-Business-using-Data-Visualization/assets/122600889/f46613c1-d53a-46e5-9240-f6eee614b459)


The data presents the cancellation ratio for two types of hotels, "City Hotel" and "Resort Hotel," across different stay duration categories. The major summary of this result indicates that:

1. For "City Hotel":

 * The cancellation ratio is relatively higher for stays lasting "3 Weeks" and ">= 4 Weeks." This suggests that longer stays are more likely to be canceled.
 * Stays with a duration of "2 Weeks" also have a relatively high cancellation ratio.
 * Stays of "<= 1 Week" have a lower cancellation ratio, indicating that shorter stays are less likely to be canceled.

2. For "Resort Hotel":

 * Similar to the "City Hotel," longer stays ("3 Weeks" and ">= 4 Weeks") have a higher cancellation ratio.
 * Stays of "2 Weeks" also have a higher cancellation ratio compared to shorter stays.
 * Stays of "<= 1 Week" have the lowest cancellation ratio, suggesting that shorter stays are less prone to cancellations.

from my assumptions, there's some reasons on why this is happening:
* **Business vs. Business Leisure**: "City Hotel" may attract more business travelers who might have uncertain schedules, leading to a higher likelihood of cancellations. On the other hand, "Resort Hotel" guests may consist of more leisure travelers who plan their vacations more firmly.

* **Seasonal Influences**: Both hotel types experience a decrease in cancellation ratios as the length of stay increases. This pattern could be due to seasonal effects, as longer stays might coincide with peak vacation seasons when travelers are less likely to cancel their reservations.


Overall, this analysis reveals a pattern where longer stay durations are associated with higher cancellation ratios for both types of hotels. It also highlights that shorter stays, especially those lasting "<= 1 Week," have a lower likelihood of being canceled. The findings can be valuable for hotel management in understanding the relationship between stay duration and booking cancellations.

## Impact Analysis of Lead Time on Hotel Bookings Cancellation Rate

Insight and Assumptions from the Plot:

![image](https://github.com/riyouuyt/Investigate-Hotel-Business-using-Data-Visualization/assets/122600889/de760468-331f-4826-94ed-d5cb078d4f24)

The data reveals a compelling relationship between lead time (booking interval) and cancellation ratios for "City Hotel" and "Resort Hotel." 📊

**Insight:**

* Shorter Lead Time, Lower Cancellation Ratio: Both hotel types exhibit a consistent pattern where decreasing lead time corresponds to lower cancellation ratios. For instance, "City Hotel" experiences its highest cancellation ratio when bookings are made 11-12 months in advance (58.6%), decreasing for lead times within one month (19.6%).

* Variations between Hotel Types: "City Hotel" generally maintains a higher cancellation ratio compared to "Resort Hotel," regardless of lead time. "Resort Hotel" enjoys a lower cancellation ratio for bookings more than 12 months ahead (17.0%), but this ratio increases as lead time shortens.

**Assumptions and Implications:**

* **Booking Confidence and Planning**: It is likely that guests booking well in advance may harbor some uncertainty about their travel plans, leading to higher cancellation rates. Conversely, guests with lead times of one month or less may have more concrete plans and thus exhibit lower cancellation ratios
* **Business and Leisure Travel**: "City Hotel" may cater more to business travelers who tend to plan trips closer to the travel date, resulting in a higher cancellation ratio. On the other hand, "Resort Hotel" attracts leisure travelers who plan ahead, showing a lower cancellation ratio.
* **Pricing and Policies**: Differences in cancellation policies, pricing strategies, or the types of market segments targeted by the hotels could contribute to the variations in cancellation ratios. Further analysis of these factors is required to gain a more comprehensive understanding of the observed trends. 💼🏖️💰




