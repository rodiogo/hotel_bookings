# Hotel_Booking 

#Business Understanding
The cancellation of the booking depends on several factors. iHolSCTEday intends to predict, based on its historical data, whether or not a customer will cancel their reservation, in order to keep their chain always full through over-overbooking.
For the business, offering the option to cancel a booking potentially generates more demand and helps anticipate occupancy. The customer has more confidence to make the reservation, in addition to a safety net in situations such as flight delays. However, the costs borne by the hotel due to cancellations are unoccupied rooms and discounted room prices, leading to reduced profits. Hotels also bear additional costs associated with overbooking (relocation costs, cash or service compensation, and social reputation).
Therefore, it is important for stakeholders to minimize the booking cancellation rate in order to make a greater profit, and maximize the number of available rooms in the hotel. The best way to gain occupancy is to make predictions using machine learning so we know who will cancel the order in advance, in order to avoid loss of profit.

#Data Understanding 
This dataset consists of guest booking information from one of the major hotel chains. The information provided should be used to build some predictive models to classify whether or not a hotel reservation will be canceled, which can affect the revenue stream.

As colunas têm a seguinte composição:  
#   Column                          Non-Null Count   Dtype   
---  ------                          --------------   -----   
0	Unnamed: 0                      119390 non-null  int64  discreta 
1	hotel                           119390 non-null  object nominal 
2	is_canceled                     109839 non-null  float64 nominal 
3	lead_time                       119390 non-null  int64  discreta 
4	arrival_date_year               119390 non-null  int64  discreta 
5	arrival_date_month              119390 non-null  object nominal 
6	arrival_date_week_number        119390 non-null  int64  discreta 
7	arrival_date_day_of_month       119390 non-null  int64  discreta 
8	stays_in_weekend_nights         119390 non-null  int64  discreta 
9	stays_in_week_nights            119390 non-null  int64  discreta 
10	adults                          119390 non-null  int64  discreta 
11	children                        119386 non-null  float64 discreta 
12	babies                          119390 non-null  int64  discreta 
13	meal                            119390 non-null  object ordinal 
14	country                         118902 non-null  object nominal 
15	market_segment                  119390 non-null  object nominal 
16	distribution_channel            119390 non-null  object nominal 
17	is_repeated_guest               119390 non-null  int64  nominal 
18	previous_cancellations          119390 non-null  int64  discreta 
19	previous_bookings_not_canceled  119390 non-null  int64  discreta 
20	reserved_room_type              119390 non-null  object nominal 
21	assigned_room_type              119390 non-null  object nominal 
22	booking_changes                 119390 non-null  int64 discreta  
23	deposit_type                    119390 non-null  object deposit type nominal 
24	agent                           103050 non-null  float64 nominal 
25	company                         6797 non-null    float64 nominal 
26	days_in_waiting_list            119390 non-null  int64  discreta 
27	customer_type                   119390 non-null  object nominal 
28	adr                             119390 non-null  float64 contínua 
29	required_car_parking_spaces     119390 non-null  int64  discreta 
30	total_of_special_requests       119390 non-null  int64  discreta 
31	reservation_status              119390 non-null  object nominal 
32	reservation_status_date         119390 non-null  object ordinal 

There are 119390 rows/notes and 33 columns.
The country, company, is_canceled, agent, children columns are the only ones with null values. The percentage of nulls per columns is company 94.31%, is_canceled 8%, agent 13.69%, children 0%, country 0.41%.

![image](https://user-images.githubusercontent.com/32617055/197893809-c224954d-92e7-4249-a3b3-5add5e1f2b1d.png)


