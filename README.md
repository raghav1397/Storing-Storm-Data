# Storing Storm Data

Recently, the International Hurricane Watchgroup (IHW) has been asked to update their analysis tools. Because of the increase in public awareness of hurricanes, they are required to be more diligient with the analysis of historical hurricane data they share across the organization. They have asked you, someone with experience in databases, to help work with their team to productionize their services.

Accepting the job, their team tells you that they have been having trouble sharing data across the teams and keeping it consistent. From what they've told you, it seems that their method of sharing the data with their data anaylsts has been to save a CSV file on their local servers and have every data analyst pull the data down. Then, each analyst uses a local SQLite engine to store the CSV, run their queries, and send their results around.

From what they have told you, you might be thinking that this is an inefficient way of sharing data. To understand what you will be working on, they have sent you a CSV file. Their CSV file contains the following fields:

    fid - ID for the row
    year - Recorded year
    month - Recorded month
    day - Recorded date
    ad_time - Recorded time in UTC
    btid - Hurricane ID
    name - Name of the hurricane
    lat - Latitude of the recorded location
    long - Longitude of the recorded location
    wind_kts - Wind speed in knots per second
    pressure - Atmospheric pressure of the hurricane
    cat - Hurricane category
    basin - The basin the hurricane is located
    shape_leng - Hurricane shape length

In this Guided Project, you will be using the local installed version of Postgres you installed from the previous project. This is much different than previous Guided Projects as you will be using your own notebook and your own Python environment instead of Dataquest's. Your job is to show that you can create a database that will accomplish the following requirements:

    Database for the IHW to store their tables.
    Table that contains the fields detailed in the CSV file
    User that can update, read, and insert into a table of the data.
    Insert the data into the table.
