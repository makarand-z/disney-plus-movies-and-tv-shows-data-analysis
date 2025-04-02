# Disney Movies and TV Shows Data Analysis 

#### This project uses PySpark for data analysis particularly focusing on data cleaning, data aggregation and reporting for extracting insights

### Data Overview
The dataset used in this project includes movie and series information with the following columns:
- imdb_id: Unique identifier for each movie
- title: Movie title
- plot: Description of the movie plot
- type: Genre of the movie
- rated: Movie's rating
- year: Year the movie was released
- released_at: Release date
- runtime: Duration of the movie
- genre: Categories the movie falls under (Action, Comedy, etc.)
- director: Director of the movie
- writer: Writer of the movie
- actors: Cast of the movie
- language: Language of the movie
- country: Country where the movie was made
- awards: Awards won by the movie
- metascore: Movie's metascore rating
- imdb_rating: IMDb rating of the movie
- imdb_votes: Number of votes on IMDb

### Aggregations and Transformations
Some of the transformations and aggregations include:

#### Handling Missing Values:
- Checked the number of missing (null) values for each column.
- Used conditional expressions (```when```) to identify and replace missing values.

#### Average IMDb Rating:
- Grouped movies by various attributes and calculated average IMDb ratings.
- Used ```groupBy``` and ```agg``` functions to compute and round the ratings for movies with or without awards.

#### Categorizing Movies Based on Awards:
- Created a new column to classify movies based on whether they won awards or not.

#### Reordering Columns:
- Reordered columns to make the data easier to interpret and display results with clear and business-friendly naming conventions.

#### Data Filtering:
- Applied filters to select movies based on their IMDb ratings.
- Performed data transformation using the ```cast``` function for type conversions.
