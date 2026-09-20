# Movie Recommendation System

## About the Project

This project is a movie recommendation system developed for Week 03 of the EncoderX AI/ML internship.

The system recommends movies based on the similarity between their genres. A content-based filtering approach is used to generate the recommendations.

## Dataset

The MovieLens dataset was used for this project.

The dataset contains movie information and user ratings. The movie data includes movie IDs, titles, and genres, while the ratings data includes user IDs, movie IDs, ratings, and timestamps.

Dataset: MovieLens Latest Small Dataset

## Data Preparation

The following steps were performed:

- Checked missing values
- Removed records with missing movie titles or genres
- Checked duplicate records
- Selected relevant columns
- Cleaned the genre information
- Prepared user-item interaction data
- Created a user-item matrix

## Recommendation Method

Content-based filtering was used for the recommendation system.

TF-IDF was used to convert movie genres into numerical features. Cosine similarity was then used to compare movies.

The movies with the highest similarity scores are returned as recommendations.

## Evaluation

The system was evaluated using Precision@5.

A total of 10 movies were tested.

Average Precision@5:

**1.0**

The score is based on the relevance condition used in this project, where a recommended movie is considered relevant if it shares at least one genre with the selected movie.

## Demonstration

A simple Gradio interface was created for testing the recommendation system.

The user can enter a movie title and select the number of recommendations. The system then displays the recommended movies with their similarity scores.

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- TF-IDF
- Cosine Similarity
- Gradio
- Google Colab

## Project Files

- `Week_03_Movie_Recommendation_System.ipynb` - Complete project notebook
- `README.md` - Project documentation

## Result

The recommendation system successfully generated movie recommendations and was tested through the Gradio interface.
