# Investigating_Netflix_Movies
## Netflix Movie Exploration with Pandas and Matplotlib

This repository explores movie data from Netflix, focusing on movie duration, genre distribution, and trends across release years. 

**Data Source:**

The data for this analysis is expected to be in a CSV file named "netflix_data.csv". This file should contain attributes like title, type (movie/show), genre, release year, and duration.

**Code Structure:**

The provided Python script (`[script_name.py]`) utilizes pandas for data manipulation and visualization, and matplotlib for creating charts. The script is organized into three sections:

1. **Data Preparation:**
    * Imports pandas and matplotlib libraries.
    * Reads the "netflix_data.csv" file into a pandas DataFrame.
    * Filters the data for movies only and selects relevant columns (title, country, genre, release year, duration).
    * Creates a subset of movies with duration less than 60 minutes (optional analysis).
    * Defines a list of important genres for further exploration ("Children", "Documentaries", "Stand-Up").

2. **Visualization 1: Movie Duration vs. Release Year**
    * Creates a scatter plot with release year on the x-axis and duration on the y-axis.
    * Assigns colors to data points based on their genre for visual distinction.

3. **Visualization 2 & 3: Genre Analysis based on Release Year**
    * Filters movies for the pre-defined list of important genres.
    * **Visualization 2.1:** Calculates the average movie duration for each genre across release years using pivot tables.
        * Creates a line plot showing the average duration trend for each genre.
    * **Visualization 2.2:** Creates a pivot table to count the number of movies for each genre in each release year.
        * Generates a line plot with release year on the x-axis and separate lines for each genre, representing the movie count for that genre in each year.

**Running the Script:**

1. Ensure you have pandas and matplotlib libraries installed (`pip install pandas matplotlib`).
2. Place the script (`[script_name.py]`) and the data file ("netflix_data.csv") in the same directory.
3. Run the script from your terminal using `python [script_name.py]`.

**Expected Output:**

The script will generate three visualizations:

1. A scatter plot depicting movie duration distribution across release years, colored by genre.
2. A line plot showing the average movie duration trend for each genre over release years.
3. A line plot showcasing the number of movies released for each genre across different release years.

**Further Exploration:**

This code provides a basic framework for exploring movie data on Netflix. You can modify the script to:

* Analyze additional genres.
* Explore relationships between movie duration, genre, and other attributes.
* Create different visualizations based on your interests.

Feel free to adapt and extend this code for further analysis of the Netflix movie data!

