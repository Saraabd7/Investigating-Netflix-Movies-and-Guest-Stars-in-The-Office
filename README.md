# Investigating-Netflix-Movies-and-Guest-Stars-in-The-Office

## Python projects on DataCamp

Apply the foundational skills in Introduction to Python and Intermediate Python courses to manipulate and visualize movie and TV data.

## Description
In these projects, I’ll apply the skills I learned in Introduction to Python and Intermediate Python to solve a real-world data science problem. I’ll press “watch next episode” to discover if Netflix’s movies are getting shorter over time and which guest stars appear in the most popular episode of "The Office", using everything from lists and loops to pandas and matplotlib.

## Guided project
Dig into a real-world Netflix movie dataset using everything from lists and loops to pandas and matplotlib.

## Project tasks:
###  - Task 1: Loading a friend's data into a dictionary.
1- Use our friend's data to create a dictionary. To do so, you will need to perform the following steps.
2- Create a list of years from 2011 to 2020 and a list durations of the average movie lengths our friend provided (103, 101, 99, 100, 100, 95, 95, 96, 93, and 90).
3- Create a dictionary movie_dict, with the keys "years" and "durations" and the values set to your lists years and durations.
4- Print and inspect the dictionary to ensure it was created correctly.

### - Task 2: Creating a DataFrame from a dictionary.
1- Import pandas using its usual alias, pd.
2- Create a DataFrame durations_df using your movie_dict dictionary you created in the previous step.
3- Print the entire DataFrame.


### -  Task 3: A visual inspection of our data.
1- Import matplotlib.pyplot under the alias plt.
2- Create a line plot of the data with the years column of durations_df on the x-axis, and the durations column on the y-axis.
3- Add the title "Netflix Movie Durations 2011-2020" to your plot.

### - task 4: Loading the rest of the data from a CSV.
1- Create another DataFrame, netflix_df, this time using the CSV file our friend provided us with, available at the path "datasets/netflix_data.csv".
2- Print the first five rows of the DataFrame to inspect the data and ensure it was created successfully.

### - Task 5: Filtering for movies!.
1- Subset the netflix_df DataFrame such that only rows where the type is a "Movie" are preserved. Assign the result to netflix_df_movies_only.
2- Subset the netflix_df_movies_only DataFrame to preserve only the columns title, country, genre, release_year, and duration. Assign the result to netflix_movies_col_subset.
3- Print the first five rows of netflix_movies_col_subset.


### - Task 6: Creating a scatter plot.

1- Using your netflix_movies_col_subset DataFrame, create a scatter plot, placing the release_year on the x-axis and the movie duration on the y-axis.
2- Add a title to your plot: "Movie Duration by Year of Release".
3- Show the plot.

### - Task 7: Digging deeper
1- Subset netflix_movies_col_subset to create a new DataFrame short_movies containing only movies that have a duration fewer than 60 minutes.
2- Print the first 20 rows of short_movies to get a good overview of the types of films with a short duration.


### - Task 8:  Marking non-feature films.

1- Initialize an empty list called colors to store our different color values.
2- Use a for loop to iterate through the netflix_movies_col_subset DataFrame's rows and append colors to your colors list based on the following conditions:
3- If the genre is "Children", append "red".
4- If the genre is "Documentaries", append "blue".
5- If the genre is "Stand-Up", append "green".
6- If the genre is any other genre, append "black".
7- Print the first 10 values of your colors list to inspect the results.


### - Task 9: Plotting with color!.
1- Using the data contained in netflix_movies_col_subset, plot the same scatter plot as you did in Task 6, but with a few modifications:
2- Color the points on the scatter plot using your colors list you defined in the previous step.
3- Add a title "Movie duration by year of release", an x-axis label "Release year", and a y-axis label "Duration (min)".
4- Show the plot.
