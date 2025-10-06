# Netflix-Analysis-Dashboard-Project

# Overview
This project involves creating a Power BI dashboard to analyze and visualize data from a Netflix dataset. The dashboard provides insights into Netflix's content library, including trends in show additions, ratings, genres, and more.

# Dataset
The dataset is sourced from a CSV file containing the following columns:

show_id: Unique identifier for each show.

type: Indicates whether it is a movie or TV show.

title: Title of the show.

date_added: Date when the show was added to Netflix.

release_year: Year when the show was released.

rating: Rating of the show.

duration: Duration of the show.

duration_type: Indicates minutes for a movie and seasons for a TV show.

cast: List of cast members.

countries: List of countries where the show was produced.

description: Brief description of the show.

directors: List of directors.

listed_in: Genres of the show.


# Data Preparation


Data Cleaning and Transformation:

Used Excel's text-to-column functionality to split entries in cast, countries, directors, and listed_in columns.
Saved transformed columns as separate CSV files.
Replaced empty cells with NULL values.


Database Setup:

Created a MySQL schema.

Converted CSV file encoding from UTF-8 to ANSI.

Imported CSV data into MySQL tables.

Power BI Dashboard

Connecting to Data:

Connected Power BI to MySQL database.

Imported relevant tables for analysis.


# Dashboard Pages:

Overview Page:

Area Chart: Trend of shows added to Netflix over the years (post-2012).

Stacked Column Chart: Distribution of shows by rating and type.

Clustered Bar Chart: Count of shows by genre.

Map: Geographic distribution of shows.


Single Title View Page:
Slicer: Select specific movie/show by title.
Cards: Display details (release year, rating, description).
Map: Show country of origin.
Multirow Cards: Display genres, cast, directors.
