# Movie Recommendation System

This Python script implements a movie recommendation system based on content-based filtering. The recommendation system suggests movies similar to a given movie title based on features such as keywords, cast, genres, and director.

## Overview

The recommendation system follows these steps:

1. **Read CSV File**: The script reads movie data from a CSV file named "movie_dataset.csv" using the pandas library.

2. **Select Features**: It selects specific features such as keywords, cast, genres, and director from the dataset.

3. **Combine Features**: It combines the selected features into a single column named "combined_features".

4. **Create Count Matrix**: Using CountVectorizer from scikit-learn, it creates a count matrix from the combined features column.

5. **Compute Cosine Similarity**: The script computes the cosine similarity between movies based on the count matrix.

6. **Get Index of Movie**: It retrieves the index of a given movie title (in this case, "Avatar").

7. **Find Similar Movies**: Based on the similarity scores, it finds similar movies to the given movie.

8. **Print Similar Movies**: It prints the titles of the first 50 similar movies in descending order of similarity score.

## Usage

To use the Movie Recommendation System:

1. Ensure you have the required dependencies installed (`pandas`, `numpy`, `scikit-learn`).
2. Place the CSV file containing movie data ("movie_dataset.csv") in the same directory as the script.
3. Run the script (`movie_recommendation_system.py`) to generate movie recommendations.
4. Input a movie title when prompted to get recommendations for similar movies.

## Requirements

- Python 3.x
- `pandas`, `numpy`, `scikit-learn` libraries

## Contributing

Contributions to enhance the movie recommendation system, add new features, or fix issues are welcome! Please feel free to submit pull requests or open issues if you encounter any problems.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
