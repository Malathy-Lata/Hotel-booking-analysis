# Hotel-booking-analysis
Objective

A hotel bookings dataset was provided for analysis. The main objective of the hotel booking analysis is to perform an Exploratory Data Analysis on the 
dataset to understand the various trends in hotel bookings and what factors govern hotel booking.


Data Summary

Total number of rows in data: 119390

Total number of columns: 32

Types of datatype in the dataset: int64, float64, and object

The given dataset of hotel bookings contains booking information for a city hotel and resort hotel respectively and various other attributes related to hotel booking


Data Wrangling

1. Handling null values

 Null values in column country were replaced by 'others'.

 Null values in columns company, children, and agent were replaced by 0.

2. Converting columns to appropriate data types

 Changed data type of children, company, and agent to int type.

 Changed data type of reservation_status_date to date type.

3. Removing outliers

 One outlier was found in the ADR column and the corresponding row was dropped from the dataset.

4. Creating new columns

 Created a new column total_stay by adding stays_in_weekend_nights and stays_in_week_nights. 

 Created a new column total_people by adding adults, children, and babies. 

 Created a new column total_kids by adding children and babies

5. Deleting certain rows

 There were rows with 0 people in the total_people column, hence dropped the corresponding rows


Exploratory Data Analysis

Performed EDA and tried answering the following questions:

1. What is the percentage of bookings for each hotel type?

2. What is the percentage of bookings for each year?

3. Which meal type is mostly preferred meal by the customers?

4. Does the customers require any car parking spaces or not?

5. What is the number of bookings made with special requests?

6. From which country most of the guests are coming?

7. Which agent makes the most number of bookings?

8. Which types of customers mostly make bookings?

9. How many people were present in a particular booking?

10. How long do people stay at the hotels?

11. Which room type is in most demand and which room type generates the highest ADR?

12. What is the preferred stay length for each hotel type?

13. Which hotel has a high chance that its customer will return for another stay?

14. Does not allotting the same room as demanded affect ADR? 

15. Which hotel is much busier and seems to make more revenue?

16. Which is the most common distribution channel and market segment for booking hotels?

17. Which channel is contributing to generating higher ADRs?

18. Which are the busiest months and which month generates higher revenue?

19. What is the trend of bookings within a month?

20. Which hotel has a higher bookings cancellation rate?

21. Which significant distribution channel and market segment have the highest cancellation percentages?

22. Does the deposit affect the cancellation of bookings?

23. Does a longer waiting period or longer lead time causes the cancellation of bookings?

24. What is the relation between the following factors and receiving special requests:

 Hotel Type

 Presence of kids and adults

 Country

 Distribution channel and market segment

 Arrival Month

 Waiting period

 Lead time

25. What is the optimal stay length for the customers in terms of ADR? What is the relationship between the following factors and ADR affecting the optimal stay:

 Lead Time

 Total People

 Waiting Period


The analysis was mainly performed using Matplotlib and Seaborn libraries, and the following graphical representation has been used:

 Correlation Heatmap

 Scatter Plot

 Box Plot

 Bar Plot

 Pie Chart

 Line Plot

 Density Plot


Correlation

 is_canceled and lead time have a slight correlation. This means that the higher the lead time of the customer the higher the cancellation rate.

 is_repeated_guest and previous_bookings_not_canceled show a slight positive correlation as it is obvious that with no previous cancellations the guest would be a repeated one

 ADR is slightly correlated with total_people, which makes sense as more people means more revenue and therefore more ADR.


Conclusion

1. The majority of the bookings from the dataset are from the year 2016.

2. Of the bookings and cancellations made, the majority of them were for a city hotel.

3. Most of the bookings made were from the European countries, predominantly from Portugal while the higher average special requests were received from African countries.

4. Bed and Breakfast was the most preferred meal type and the majority of the guests had no requirement for car parking spaces.

5. For a shorter stay length (less than 5 days) city hotels are predominant, whereas for longer stay length (greater than 7 days) resort hotels are preferred.

6. Guests used different channels for booking their stay and among them, the preferred way is TA/TO. Also, the majority of the cancellations were made via channel TA/TO.

7. Hotels can work to increase outreach on GDS channels to get higher revenue-generating deals

8. The bookings made via TA/TO channel are booked way ahead of the actual arrival date.

9. Cancellation of bookings is not affected by not getting the same room as reserved, deposit type, longer lead time, and waiting time. Although a slightly lesser ADR is observed for bookings with a different room allotted than the reserved one.

10. July and August are the busier and most profitable months for both hotels.

11. Within a month, for both hotels, arrival increases during weekends and ADR gradually increases as the month ends.

12. Most of the special requests are received by the city hotel and from the channel TA/TO. In July - August most of the requests were received. More number of people (kids and adults) in a particular booking results in more number of special requests.

13. For customers, generally, longer stays (more than 15 days) can result in better deals in terms of low ADR.


Challenges

1. Data was present in the wrong datatype format

2. Choosing appropriate visualization techniques to use was difficult.

3. A lot of null values were there in the dataset.
