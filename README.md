This project aims to predict the movie rating based on several features, such as the movie's genre, director, actors, duration, and more. The data used in this project contains multiple attributes of movies, including:

Name: The title of the movie.

Year: The release year of the movie.

Duration: The runtime of the movie.

Genre: The genre(s) of the movie.

Rating: The IMDB rating of the movie.

Votes: The number of votes the movie received.

Director: The director(s) of the movie.

Actor 1, Actor 2, Actor 3: The main actors in the movie.

Data Preprocessing
Importing Libraries and Reading Data: We begin by importing the necessary libraries and reading the dataset.

Data Cleaning:

Handling Missing Values: Missing or null values are identified and managed.

Changing Duration and Votes to Numeric: The duration and votes columns are converted to numeric values for proper analysis.

Removing Duplicate Data: Any duplicate entries are removed to ensure data quality.

Cleaning Genre and Year Columns: The genre and year columns are cleaned to ensure consistency, and a new genre column is created for further analysis.

Distribution of Movies Across Genres: The distribution of movies across different genres is analyzed to identify trends and patterns in the data.

Data Insights
Rating and Duration Distribution:

Rating and Duration are both normally distributed, indicating that most movies have average ratings and runtimes close to the mean.

Votes:

The votes are right-skewed with many outliers, indicating a significant number of movies have an exceptionally high number of votes. These outliers are kept for prediction purposes since they are part of the real-world data.

Top 3 Genres by Movie Count:

Drama, Action, and Comedy are the top three genres with the highest number of movies.

Average Ratings by Genre: The average ratings for the main genres are as follows:

Documentary: 7.57

History: 7.23

Biography: 6.60

Sci-Fi: 6.33

Family: 6.30

Fantasy: 6.25

Drama: 6.24

Adventure: 6.13

Music: 6.12

Crime: 6.09

Animation: 6.07

Mystery: 5.82

Comedy: 5.81

Sport: 5.80

Romance: 5.59

Action: 5.51

Thriller: 5.33

Horror: 4.69

War: 4.33

Movies Over Time:

The number of movies has been increasing year over year, peaking in 2019 with 224 movies released.

Model Building and Evaluation
XGBoost Model:

The XGBoost model was used to predict movie ratings based on the various features. The model was trained and tested, achieving an R2 score of 0.86.

The model predicted a rating of 6.8 for a new movie, which is close to the true rating of 7.4 in row 10, showing the robustness of the model.

Cross-validation:

The model achieved an average score of 0.85 during cross-validation, with no significant differences between folds, indicating that the model is not overfitting.

Conclusion
The analysis and the XGBoost model provide valuable insights into movie ratings, the factors affecting them, and the overall distribution of ratings across genres. The model demonstrates a good ability to predict movie ratings, with strong performance in cross-validation and a high R2 score.
