# Flight-Status-Dashboard
Introduction to Simulated Role
In this project I will be monitoring the operational efficiency of airlines in USA based on their performance, delays and cancellations. I analysed the trends and figures in the flight
operations using the data and provided some useful insights by creating a dynamic dashboard.
Key responsibilities include:
•	Create a dynamic dashboard that can monitor status of the flights including delays and cancellations.
•	Identify which airports have consistent issues.
•	Help the decision makers to identify the issue and improve the operational efficiency.

Introduction to Data Source
The dataset used in the dashboard contains four tables – airlines, airports, cancellations codes and flights. Flights table is the fact table and one to many relationships were established to this fact table by the remaining tables creating a star schema. The data source provides us the information on airline and airport efficiency and also gives the reason behind cancellations

Initial Findings/Data Exploration
•	By using flight status, airlines and airports we can analyse the operational efficiency of the flights by city and airport.
•	Out of 2 million flights 41% of flights were delayed and 1.45% flights were cancelled.
•	Highest number of flights that were cancelled was on Monday
•	United Airlines Inc. was the airlines which had most delays.

Methodologies and Preprocessing
Data Cleaning
•	Unwanted rows were removed from the Flights table.
•	Added conditional column to get the status of the flight using delayed time column in the flights table
 
•	Promoted the headers in airlines table and cancellation code table
Data Modelling
Measures were created using DAX for:
•	Getting total number of flights, On-time flights, delayed flights and cancelled flights
•	Also calculated the percentages of On-time flights, delayed flights and cancelled flights
Visualizations
•	Bar charts were used to show the Total number of flights by each city and % delayed flights in each airport.
•	Number cards were used to show the percentages of On-time flights, delayed flights and cancelled flights
•	Line charts were used to show the percentages of On-time flights, delayed flights and cancelled flights by month
•	Donut chat was used to show the reason for cancellation and their number
•	Three slicers were made to easily navigate using moth, airline and city filters.


DEEP DIVE ANALYTICS


2.1 Delay Analytics
Most common delay cause: Carrier delays always account for the lion's share of flight delays, indicating internal airline operations inefficiencies. 

Weather delays seasonally peak (e.g., winter storms or summer thunderstorms) and are prominent in the Northeast region. 

Late aircraft delays are highly correlated with high-volume hubs (e.g., ATL, ORD, DFW), implying cascading effects from previous flights. 

2.2 Cancellation Trends
Top cancellation airports are ORD, JFK, and LAX — all major hubs with dense traffic volume and exposure to weather or congestion.

Security cancellations are rare but concentrated in a subset of airports, possibly indicating infrastructure or incident response protocols.

2.3 Geographic Insights
A map visualization shows delay and cancellation clusters:

Northeast (JFK, BOS) experiences high weather delays.

Southern and Midwest airports experience more carrier-related delays.

A more focused look at states like New York and Illinois illustrates consistent flight disruption. 

2.4 Airline Performance
Airlines witness higher-than-average delays.

Low-cost airlines may see fewer flights in total but disproportionately higher delays, likely due to pared operations.

3. Recommendations
•	Operational Improvements
Root Cause Isolation: Airports should isolate some routes or aircraft types that have a propensity for many late aircraft delays.

Schedule Buffering: Add buffer time in timetables for high-risk weather months.

Data-Driven Staffing: Airports should use historical trends of delays to enhance staffing of ground crews and security personnel for busy periods.

•	Passenger Communication
Add real-time dashboards at airports and mobile apps to inform passengers of potential delays/cancellations ahead of time.

Use predictive analytics to forecast delay probability for upcoming flights.

•	Collaboration
Airports and airlines need to collaborate on data sharing in an effort to better understand dependencies (e.g., delays in gate usage due to late arrivals).

4. Limitations and Assumptions
•	Limitations
No real-time data: Data is historic and does not reflect recent trends post-COVID or new airline policies.

No passenger data: Impact of delays/cancellations on customer satisfaction or refunds is not included.

Route-level granularity not present: Origin-destination pair analyses would be useful.

•	Assumptions
Delays' reasons are correctly labeled by reporting bodies.

Airports are treated as independent units, rather than most delays being interlinked in airport hubs.

Weather-related delays are assumed to be outside airport control and unrelated to infrastructure and airport readiness.


Future Directions


•	Increased Data
Merge real-time delay data and weather predictions to build forecasting delay models.

Integrate customer feedback metrics to connect delays with satisfaction ratings.

•	Improved Mapping
Use geospatial clustering to uncover regional inefficiency or airspace saturation.

Insert route maps of normally delayed flights between city pairs.

•	Machine Learning Uses
Build machine learning models (e.g., Random Forest or XGBoost) that forecast delay probabilities from flight characteristics.

Forecast airport congestion based on seasonal and historic trends.

•	Business Applications
Deliver airlines with custom dashboards for comparing their performance against the competition.

Deliver city and state-level views to assist policy makers in managing transportation budgets more effectively.

CONCLUSION

This project demonstrates the power of data insights to address operating challenges in the airline industry. With the analysis of historical flight data, we uncovered key trends related to flight cancellations and delays, and identifying prime causes were carrier inefficiencies and weather. The interactive dashboard provides actionable insights to airlines, airports, and regulatory authorities to improve punctuality, usage of resources, and passenger satisfaction.

In spite of dataset limitations, such as insufficient real-time feeds and passenger influence data, results still present a solid foundation for informed decision-making. By building on this effort with predictive modeling, real-time integration, and expanded datasets, stakeholders can move toward an improved proactive and resilient air transportation system.

Lastly, this project not only records the then-dominate airline performance but also creates the entry for strategic intervention and innovation in the travel system.
