# AtliQ Grands Business Intelligence Project

## Problem Definition

AtliQ Grands, a renowned luxury hotel chain, is experiencing a decline in market share and revenue due to increased competition and management inefficiencies. To counter this, the managing director has decided to leverage Business and Data Intelligence to regain market dominance. However, lacking an in-house data analytics team, they've engaged a third-party service provider to analyze their historical data.

## Data Overview
We have three dimension tables and two fact tables. Details are given below:
### Dimension Tables
1. **dim_date**:
   - date: Dates in May, June, and July.
   - mmm yy: Month and year format.
   - week no: Unique week number.
   - day_type: Weekday or Weekend.

2. **dim_hotels**:
   - property_id: Unique hotel ID.
   - property_name: Hotel name.
   - category: Luxury or Business class.
   - city: Location of the hotel.

3. **dim_rooms**:
   - room_id: Room type (RT1, RT2, RT3, RT4).
   - room_class: Room class (Standard, Elite, Premium, Presidential).

### Fact Tables
1. **fact_aggregated_bookings**:
   - property_id: Unique hotel ID.
   - check_in_date: Check-in dates.
   - room_category: Room type.
   - successful_bookings: Number of successful bookings.
   - capacity: Maximum room capacity.

2. **fact_bookings**:
   - booking_id: Unique booking ID.
   - property_id: Unique hotel ID.
   - booking_date: Booking date.
   - check_in_date: Check-in date.
   - check_out_date: Check-out date.
   - no_guests: Number of guests.
   - booking_platform: Booking platform.
   - ratings_given: Customer ratings.
   - booking_status: Booking status (Cancelled, Checked Out, No show).
   - revenue_generated: Total revenue.
   - revenue_realized: Final revenue after deductions/refunds.

## Data Pre-processing

### Calculated Measures
- Revenue
- Total Bookings
- Total Capacity
- Total Successful Bookings
- Occupancy %
- Average Rating
- No of Days
- Total Cancelled Bookings
- Cancellation %
- Total Checked Out
- Total No Show Bookings
- No Show Rate %
- Booking % by Platform
- Booking % by Room Class
- ADR (Average Daily Rate)
- Realization % (successful "checked out" percentage overall bookings)
- RevPAR (Revenue Generated per available room)
- DBRN (Daily Booked Room Nights)
- DSRN (Daily Sellable room nights)
- DURN (Daily Utilized room nights)
- Revenue WoW change %
- Occupancy WoW change %
- ADR WoW change %
- RevPAR WoW change %
- Realization WoW change %
- DSRN WoW change %

## Data Modeling
![](https://res.cloudinary.com/dymx9fvj9/image/upload/v1707306904/Data_Model_Diagram_n3bsfd.png)

## Visualizations and Insights

### Main Dashboard
![](https://res.cloudinary.com/dymx9fvj9/image/upload/v1707306904/Data_Model_Diagram_n3bsfd.png](https://res.cloudinary.com/dymx9fvj9/image/upload/v1707307978/Main_xurla1.png)

**KPI Cards:**
- Revenue
- RevPar
- DSRN
- Occupancy %
- ADR
- Realization

**Slicers:**
- By City
- By Room Class
- By Month
- By Week Number

### Additional Dashboards

## Important Insights

1. Mumbai generated the highest revenue: 660.6M.
2. The highest ratings were received by Delhi: 3.8, whereas the average brand rating is 3.62.
3. Weekends generated more revenue: 2bn.
4. AtliQ Exotica outperforms other properties with 320 Million in revenue, a rating of 3.62, an occupancy percentage of 57%, and a cancellation rate of 24.4%.
5. Elite-type rooms have the highest booking rate but also higher cancellation rates.

---

This README provides a comprehensive overview of the AtliQ Grands Business Intelligence project, including problem definition, data overview, preprocessing details, data modeling, visualizations, and key insights.
