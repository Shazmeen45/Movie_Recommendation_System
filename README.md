# Movie Recommendation System

## Project Overview

This project is a simple movie recommendation system developed as part of the EncoderX AI/ML Week 03 task.

The system recommends movies that are similar to a movie selected by the user. For this project, I used the MovieLens dataset and built a content-based recommendation system.

## Dataset

The MovieLens Latest Small dataset was used for this project.

The main files used were:

- movies.csv
- ratings.csv

The movies data contains movie titles and genres, while the ratings data contains user ratings.

## Data Preparation

The dataset was checked for missing values and duplicate records.

For the movie data:

- Missing movie titles and genres were removed.
- Duplicate records were removed.
- Only the required movie columns were kept.
- The genre separator was changed from `|` to spaces.

User-item interaction data was also prepared from the ratings dataset.

## Recommendation Approach

Content-Based Filtering was used for this project.

The recommendation system compares movies based on their genre information.

TF-IDF was used to convert the movie genres into numerical features. Cosine similarity was then used to calculate the similarity between movies.

## Recommendation Example

For example, when `Toy Story (1995)` was entered, the system recommended movies such as:

- Antz (1998)
- Toy Story 2 (1999)
- Adventures of Rocky and Bullwinkle, The (2000)
- Emperor's New Groove, The (2000)
- Monsters, Inc. (2001)

## Evaluation

The recommendation system was evaluated using Precision@5.

The system was tested on 10 movies.

Average Precision@5:

**1.00**

For this project, a recommendation was considered relevant when it shared at least one genre with the selected movie.

## Demonstration Interface

A simple Gradio interface was created for the project.

The user can enter a movie title and select the number of recommendations they want to receive.

The interface then displays the recommended movies along with their similarity scores.

## Tools and Technologies

- Python
- Google Colab
- Pandas
- NumPy
- Scikit-learn
- Gradio
- MovieLens Dataset

## Project Files

The main project notebook contains the complete implementation, including:

- Dataset loading
- Data preprocessing
- User-item interaction preparation
- TF-IDF feature extraction
- Cosine similarity
- Recommendation function
- Evaluation
- Gradio interface
