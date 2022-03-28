# Data_Lake-Project_Udacity-

The purpose of this database is to be able to extract, transform and load  different json files  that are located in different paths. For this project, there are some variables (columns headers )that are in different paths(song_data and log_data), in addition, there is some other information such as the log information that are also in a different path. With a careful study of the table, one was able to identify fact tables and dimension tables that are referenced in order to develop a logical schema. With the ETL , I was able to create relevant tables with the required information and apply the appropriate SELECT statement to transform some of the data.  The table is now a more organised version of the data instead of the different json files that are in different paths, as such the analytical teams can perform further analysis and transformation on the data to meet their different goals. 

For this particular project, the input data is transformed from AWS s3 bucket, and after the transfromation is completed, the output data is loaded back to s3. It should be noted that this process can also be performed locally.
 
The database schema here is the STAR -Schema for the following reasons:
It is simple and most widely used in the industry 
It contains one fact table and some other dimension tables that can reference each other

Please Note: I ran this project locally on my personal machine

To run the ETL
$python etl.py



Example queries
Get count of rows in each Dimension table:
SELECT COUNT(*)
FROM songs_table;
