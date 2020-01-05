## How to run whole project
1. Run 'python creat_tables.py'
2. Run  'test.ipynb'
3. restart 'test.ipynb'
4. Run 'etl.ipynb'
5. restart 'etl.ipynb'
6. Run 'python creat_tables.py' again and Run'etl.py'


## Project Analysis
1. Discuss the purpose of this database in the context of the startup, Sparkify, and their analytical goals.
The purpose of this database is to extract userful information from log data and song data for analyzing users who use music streaming app, such as what kinds of song, whether the user is using paid or free mode, where is the user located, what media they use to play songs from log data and song data. Their analytical goals are what kinds of song are most frequently played by the users.

2. State and justify your database schema design and ETL pipeline.
I created a star schema by including one fact table and  four dimension tables.Songplays table is a fact table to store song records of users use music streaming app.Four dimension tables -users, songs, artists and time, are used to store details of song records and users' information.
ELT pipeline is important step in this prokect. Becasue I have to extract data from log datasets and song datasets to build each table. However, some data formats are neccessary to transformation duing pipeling data, such as wh
3. [Optional] Provide example queries and results for song play analysis.
![Alt text](https://github.com/Waichung1015/Data-Modelling-with-Postgres/blob/master/image.png)
We can find that one song from songs table are listened by user, other songs listened by users can't find from song table.