# Disney+ Hotstar Exploratory Data Analysis (EDA)

This project is an exploratory data analysis (EDA) of the Disney+ Hotstar content dataset. Through data cleaning, visualization, and statistical insights, this analysis aims to uncover interesting patterns and trends within Disney+'s content library, including movie and show ratings, genres, runtimes, and yearly release trends.

## Dataset Overview
The dataset used in this project contains information about Disney+ Hotstar shows and movies, including fields such as IMDb ratings, runtime, genres, release year, and more. The dataset was provided as part of a master class by WsCube TECH.

### Dataset Features
- `imdb_id`: IMDb ID for each title.
- `title`: The title of the movie or show.
- `type`: Type of content (e.g., movie or show).
- `imdb_rating`: IMDb rating of the title.
- `year`: Release year.
- `genre`: Genre(s) of the title.
- `runtime`: Duration of the title in minutes.
- `language`, `country`, `director`, `actors`: Additional metadata fields.

## Project Objectives
- **Data Cleaning**: Handle missing values, convert data types, and remove irrelevant columns.
- **Data Analysis**: Explore various features to uncover trends, distributions, and relationships.
- **Data Visualization**: Use visualizations to present findings in an intuitive way.

## Data Cleaning Process
- Removed rows with missing essential information in fields like `imdb_id`, `title`, `type`, `imdb_rating`, and `year`.
- Dropped irrelevant columns with high amounts of missing data, such as `awards`, `metascore`, `writer`, `plot`, etc.
- Filled missing values in `runtime` with the median and processed string values.
- Imputed missing values in categorical columns with the most common value in each column.
- Cleaned up `imdb_votes` by removing commas and converting to numerical format.

## Key Insights from EDA
1. **IMDb Rating Distribution**: The majority of Disney+ content has IMDb ratings between 6 and 8, suggesting generally favorable content quality.
2. **Runtime Analysis**: Most titles have a runtime around 90-120 minutes, typical of movies.
3. **Content Types**: Disney+ primarily hosts movies over shows.
4. **Popular Genres**: Genres such as Drama, Comedy, and Family are the most common.
5. **Yearly Content Trends**: There has been an increasing trend in the number of releases over recent years.
6. **Correlation Analysis**: Weak correlation between IMDb rating, runtime, and IMDb votes, indicating that these factors are not strongly related.

## Visualizations
The following visualizations were created to illustrate various aspects of the Disney+ content library:
- **IMDb Rating Distribution**: Histogram displaying the spread of IMDb ratings.
- **Runtime Distribution**: Histogram showing the duration distribution of titles.
- **Content Type Count**: Bar chart showing counts of different content types.
- **Top 10 Genres**: Bar chart displaying the top genres on Disney+.
- **Yearly Release Trends**: Line plot showing the number of titles released per year.
- **Correlation Heatmap**: Heatmap visualizing the correlations between IMDb ratings, runtime, and IMDb votes.

## Getting Started
### Prerequisites
- **Python** 3.6+
- **Pandas**, **Matplotlib**, **Seaborn** for data analysis and visualization

### Running the Project
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/DisneyPlus-Hotstar-EDA.git
   cd DisneyPlus-Hotstar-EDA
