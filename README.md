# Movie_Recommendation_System

## Project Overview

1. **Data Loading**: The project loads movie data from a CSV file (`movies.csv`) into a pandas DataFrame.

2. **Data Preprocessing**: The relevant features for recommendation, namely 'genres', 'keywords', 'tagline', 'cast', and 'director', are selected. Any missing values in these features are replaced with empty strings.

3. **Feature Combination**: The selected features are combined into a single feature, 'combined_features', which represents the combined textual information of each movie.

4. **Feature Vectorization**: The textual data in 'combined_features' is converted into numerical feature vectors using the Term Frequency-Inverse Document Frequency (TF-IDF) vectorizer.

5. **Cosine Similarity**: The cosine similarity between the feature vectors of different movies is calculated. The similarity score indicates how closely related one movie is to another.

6. **User Input**: The user is prompted to enter the name of their favorite movie.

7. **Recommendation**: The system finds the closest match for the user's favorite movie from the dataset and retrieves a list of similar movies based on similarity scores.

8. **Display Recommendations**: The system displays a list of recommended movies to the user.

## Usage

1. Make sure you have the required libraries installed. If not, install them using the following command:
pip install numpy pandas scikit-learn

2. Clone this repository to your local machine.

3. Place the `movies.csv` file in the same directory as the code files.

4. Run the provided Python script to execute the movie recommendation system.

5. Enter the name of your favorite movie when prompted.

6. The system will display a list of recommended movies based on the similarity to your favorite movie.

## Note

The movie recommendation system relies on content-based filtering, which suggests movies based on their own features. It does not take into account user preferences or interactions with other users. For a more advanced recommendation system, collaborative filtering techniques or hybrid approaches could be considered.

## Acknowledgment

The dataset used in this project is provided by [www.Kaggle.com](https://www.kaggle.com/). We thank them for sharing the movie data and supporting the data science community.


