Climate Analysis and Flask API ReadMe

Congratulations on deciding to treat yourself to a long holiday vacation in Honolulu, Hawaii! To assist with your trip planning, you've chosen to conduct a climate analysis of the area. The following sections outline the steps I used to accomplish this task.

Part 1: Analyze and Explore the Climate Data
In this section, I utilized Python, SQLAlchemy, Pandas, and Matplotlib to perform a basic climate analysis and data exploration of the climate database provided.

Part 2: Design a query to get the previous 12 months of temperature observation (TOBS) data. I used the following steps:
Filter by the station that has the greatest number of observations.
Query the previous 12 months of TOBS data for that station.
Plot the results as a histogram with bins=12

Part 3:
Now that I created my initial analysis, I designed a Flask API based on the queries that I created. To do so, I use Flask to create your routes as follows:
  /
Start at the homepage.
List all the available routes.
  /api/v1.0/precipitation
Convert the query results from your precipitation analysis (i.e. retrieve only the last 12 months of data) to a dictionary using date as the key and prcp as the value.
Return the JSON representation of your dictionary.
  /api/v1.0/stations
Return a JSON list of stations from the dataset.
  /api/v1.0/tobs
Query the dates and temperature observations of the most-active station for the previous year of data.
Return a JSON list of temperature observations for the previous year.
  /api/v1.0/<start> and /api/v1.0/<start>/<end>
