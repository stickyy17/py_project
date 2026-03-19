Our project on floight data and following tasks: 

Step	Task Description		| 	SQL Techniques
-------------------------
1	Import flight schedules, passenger counts, crew assignments, and satisfaction surveys. Create unique flight identifiers and ensure all tables can be joined at flight level		| 	Multiple JOIN types, COALESCE for missing values, key generation
-------------------------
3	For each route (origin-destination pair), calculate 7-day, 30-day, and 90-day rolling average load factors. Identify routes with improving/declining demand. Calculate load factor volatility (standard deviation over rolling windows).	| 	Window AVG and STDDEV over time partitions by route
-------------------------
4	Create delay categories: on-time (<15 min), minor delay (15-60 min), major delay (60-180 min), severe delay (>180 min), cancellation. Calculate rolling on-time percentage by route and airline.	|		Date/time difference calculations, CASE for delay categories, window AVG of on-time flags
-------------------------

