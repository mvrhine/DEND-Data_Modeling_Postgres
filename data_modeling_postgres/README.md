<h1>Data Modeling with Postgres</h1>


Sparkify, a startup, is interested in analyzing songs and user activity from a new streaming app. The analytics team is interested in understanding the songs users have been listening to in the past. Currently, they do not have a easy way to query their data. So, they need a database that can organize and store JSON logs on user activity on the app, as well as a directory with JSON metadata on the songs in their app. I will create a Postgres database to optimize queries for their use case. 

<h2>Schema</h2>

Fact and dimension tables were defined for a star schema with an analytic focus.
Fact Table

songplays - records in log data associated with song plays i.e. records with page NextSong songplay_id, start_time, user_id, level, song_id, artist_id, session_id, location, user_agent
Dimension Tables

users - users in the app user_id, first_name, last_name, gender, level

songs - songs in music database song_id, title, artist_id, year, duration

artists - artists in music database artist_id, name, location, lattitude, longitude

time - timestamps of records in songplays broken down into specific units start_time, hour, day, week, month, year, weekday


</h4>Database creation<h4>

The Database creation script is used to create a database and designated tables. If you run the **python create_tables.py** file, it will do this for you.  

</h4>ETL Notebook<h5>

A Jupyter notebook will be provided to show the step by step ETL process. 
