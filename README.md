The project features three stages:

1. Familiarize yourself with the business context. Use SQL to extract a customer dataset. Explore the data at different levels of aggregation and form a plan for further analysis.
2. Make calculations related to the business context then segment customer behavior data with statistical and visual techniques using the appropriate tools.
3. Create an executive summary and slides of the customer segmentation results and record a video presentation.

Project Motivation

What is segmentation? 

It refers to a broad category of analytic techniques that allow us to group similar data points. In this project, data points will represent customers, who we will group according to their shopping behavior in the context of a very specific business initiative.

TravelTide 

e-booking startup TravelTide is a hot new player in the online travel industry. It has experienced steady growth since it was founded at the tail end of the covid pandemic (2021-04) on the strength of its data aggregation and search technology, which is best in class. Customer feedback has shown, and industry analysts agree, TravelTide customers have access to the largest travel inventory in the e-booking space. 

The perks most likely to attract customers are:
• free hotel meal
• free checked bag
• no cancellation fees
• exclusive discounts
• 1 night free hotel with flight

You can find a description of each table and its columns below:
 
1.) users: user demographic information

    * user_id: unique user ID (key, int)
    
    * birthdate: user date of birth (datetime)
    
    * gender: user gender (nominal)
    
    * married: user marriage status (binary)
    
    * has_children: whether or not the user has children (binary)
    
    * home_country: user’s resident country (nominal)
    
    * home_city: user’s resident city (nominal)
    
    * home_airport: user’s preferred hometown airport (nominal)
    
    * home_airport_lat: geographical north-south position of home airport (decimal)
    
    * home_airport_lon: geographical east-west position of home airport (decimal)
    
    * sign_up_date: date of TravelTide account creation (datetime)
    
2.) sessions: information about individual browsing sessions (note: only sessions with at least 2 clicks are included)

    * session_id: unique browsing session ID (key, string)
    
    * user_id: the user ID (foreign key, int)
    
    * trip_id: ID mapped to flight and hotel bookings (foreign key, string)
    
    * session_start: time of browsing session start (timestamp)
    
    * session_end: time of browsing session end (timestamp)
    
    * flight_discount: whether or not flight discount was offered (binary)
    
    * hotel_discount: whether or not hotel discount was offered (binary)
    
    * flight_discount_amount: percentage off base fare (decimal)
    
    * hotel_discount_amount: percentage off base night rate (decimal)
    
    * flight_booked: whether or not flight was booked (binary)
    
    * hotel_booked: whether or not hotel was booked (binary)
    
    * page_clicks: number of page clicks during browsing session (int)
    
    * cancellation: whether or not the purpose of the session was to cancel a trip (binary)
    
3.) flights: information about purchased flights

    * trip_id: unique trip ID (key, string)
    
    * origin_airport: user’s home airport (nominal)
    
    * destination: destination city (nominal)
    
    * destination_airport: airport in destination city (nominal)
    
    * seats: number of seats booked (int)
    
    * return_flight_booked: whether or not a return flight was booked (binary)
    
    * departure_time: time of departure from origin airport (timestamp)
    
    * return_time: time of return to origin airport (timestamp)
    
    * checked_bags: number of checked bags (int)
    
    * trip_airline: airline taking user from origin to destination (nominal)
    
    * destination_airport_lat: geographical north-south position of destination airport (decimal)
    
    * destination_airport_lon: geographical east-west position of destination airport (decimal)
    
    * base_fare_usd: pre-discount price of airfare (decimal)
    
4.) hotels: information about purchased hotel stays

    * trip_id: unique trip ID (key, string)
    
    * hotel_name: hotel brand name (nominal)
    
    * rooms: number of rooms booked with hotel (int)
    
    * check_in_time: time user hotel stay begins (timestamp)
    
    * check_out_time: time user hotel stay ends (timestamp)
    
    * hotel_per_room_usd: pre discount price of hotel stay (decimal)

The reference file:

1.) spreadsheet: https://docs.google.com/spreadsheets/d/13k18sEXmxbXBz1QkGiz0Kl7rHTjObEAtnClM0R7tD5Q/edit#gid=1283280955


