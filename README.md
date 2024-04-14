# Investigating_Netflix_Movies
## Netflix Movie Exploration with Pandas and Matplotlib

This repository explores movie data from Netflix, focusing on movie duration, genre distribution, and trends across release years. 

**Data Source:**

The data for this analysis is expected to be in a CSV file named "netflix_data.csv". This file should contain attributes like title, type (movie/show), genre, release year, and duration.

**Code Structure:**

The provided Python script (`[Investigating_Netflix_Movies]`) utilizes pandas for data manipulation and visualization, and matplotlib for creating charts. The script is organized into three sections:

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
3. Run the script from your terminal using `python [Investigating_Netflix_Movies]`.

**Expected Output:**

The script will generate three visualizations:

1. A scatter plot depicting movie duration distribution across release years, colored by genre.
   ![image](https://github.com/Red-54/Investigating_Netflix_Movies/assets/128955905/509f9984-1a54-4133-8d35-02f0e7306091)
   Looking at the scatter plot, we can observe a few trends:

   **Genre and Release Year**: Stand-up comedies (yellow) seem to be concentrated in more recent release years (farther right on the x-axis), whereas children's movies (red) show a wider spread across years. This might suggest a rise in stand-up comedy content on Netflix in recent times.
   
   **Genre and Duration**: There seems to be a wider spread of durations for documentaries (blue) compared to children's movies (red) and stand-up comedies (yellow). Documentaries might encompass a larger variety of short and long formats, while children's movies and stand-up comedies tend to have shorter durations on average.

3. A line plot showing the average movie duration trend for each genre over release years.
   ![image](https://github.com/Red-54/Investigating_Netflix_Movies/assets/128955905/1c758096-17f3-4686-b276-9f134d4a8521)
   The data suggests some interesting trends:
   
   **Children's Content**: There might be an increase in the duration of children's content around 1990. It's worth investigating if this coincides with a specific shift in children's programming or media formats.

   **Documentaries**: The graph reveals how documentary lengths have changed over time.Before 1990's the duration was very great after it started fluctuating towards shorter duration

5. A line plot showcasing the number of movies released for each genre across different release years.
   ![image](https://github.com/Red-54/Investigating_Netflix_Movies/assets/128955905/fe250947-fffd-411f-9bde-0610a8e72380)

   This graph shows the number of titles on Netflix by genre and release year. The data suggests that the number of titles in all genres has **increased** over time.  **Documentaries** appears to be the most **explosive** genre on Netflix, with the number of titles in this genre increasing significantly in recent years. The number of **Children's Movies** on Netflix has also grown steadily over time. **Stand-Up comedy** are the **least common** on Netflix, but the number of titles in this genre has also increased in recent years.
   

**Further Exploration:**

This code provides a basic framework for exploring movie data on Netflix. You can modify the script to:

* Analyze additional genres.
* Explore relationships between movie duration, genre, and other attributes.
* Create different visualizations based on your interests.

Feel free to adapt and extend this code for further analysis of the Netflix movie data!

