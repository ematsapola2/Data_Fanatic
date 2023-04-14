# Data_Fanatic


/****** Script for SelectTopNRows command from SSMS  ******/
SELECT *
  FROM [SQL Tutorials3].[dbo].[cycle_hire]


  SELECT count(*) AS num_of_Trips
  FROM [SQL Tutorials3].[dbo].[cycle_hire]
  WHERE duration >= 1200


  SELECT start_station_name, end_station_name, bike_id
   FROM [SQL Tutorials3].[dbo].[cycle_hire]
   WHERE bike_id = 1710


   SELECT count(distinct bike_id) AS num_bikes
   FROM [SQL Tutorials3].[dbo].[cycle_hire]
   WHERE end_station_name = 'Moor Street, Soho'

   SELECT Distinct start_station_id
   FROM [SQL Tutorials3].[dbo].[cycle_hire]
   WHERE start_station_id = 'Canton Street, Poplar'


   SELECT Distinct start_station_name
   FROM [SQL Tutorials3].[dbo].[cycle_hire]
   WHERE bike_id = 111


   SELECT count(distinct bike_id)
   FROM [SQL Tutorials3].[dbo].[cycle_hire]
   WHERE duration > 2400


   SELECT start_station_name
   FROM [SQL Tutorials3].[dbo].[cycle_hire]
   WHERE start_station_name IN ('Ram Street, Wandsworth', 'Park Lane , Hyde Park') 


   SELECT start_station_name
   FROM [SQL Tutorials3].[dbo].[cycle_hire]
   WHERE start_station_name = 'Ram Street, Wandsworth' OR start_station_name = 'Park Lane , Hyde Park'


    SELECT start_station_name
   FROM [SQL Tutorials3].[dbo].[cycle_hire]
   WHERE duration >500 AND bike_id between 300 AND 1000 



   SELECT start_station_name
   FROM [SQL Tutorials3].[dbo].[cycle_hire]
   WHERE start_station_name LIKE 'C%S%'

