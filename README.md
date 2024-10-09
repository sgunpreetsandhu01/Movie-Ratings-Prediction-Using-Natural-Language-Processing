# Movie Ratings Prediction using Natural Language Processing (NLP)



## Project Overview

This project aims to predict user ratings for movies based on features extracted from movie titles, genres, and user ratings. The project utilizes various machine learning models to achieve this goal, including Linear Regression, Random Forest Regression, and an Artificial Neural Network (ANN) Regression. The dataset combines movie metadata with user rating data, and techniques such as natural language processing (NLP) and dimensionality reduction are applied to enhance the predictive power of the models.

## Project Workflow

### 1. Data Preprocessing
- **Dataset Combination:** 
  - Two datasets were merged: one containing movie titles, genres, and movie IDs, and the other containing user ratings and user IDs.
- **Feature Engineering:**
  - The dataset was enhanced by extracting the release year from the movie title and encoding movie genres into separate columns.
- **Text Processing with NLP:**
  - Tokenization and Word2Vec embedding techniques were applied to convert movie titles into numerical vectors for model input.
  - Dimensionality reduction using PCA was performed to reduce the vector size from 100 dimensions to 2 dimensions, improving computational efficiency.
- **Final Dataset Preparation:**
  - One-hot encoding was applied to categorical features, and the dataset was split into training and test sets.

### 2. Model Training
Three machine learning models were trained to predict movie ratings:
- **Linear Regression**
- **Random Forest Regression**
- **Artificial Neural Network (ANN) Regression**

### 3. Results
The models were evaluated on a validation set, and the results were as follows:
- **Linear Regression:** Accuracy of 0.8411
- **ANN Regression:** Accuracy of 0.8125

For leaderboard predictions, the following results were obtained:
- **Linear Regression:** Score of 89
- **ANN Regression:** Score of 88
- **Random Forest Regression:** Score of 93

The ANN performed the best overall, but due to the simplicity and competitive performance of Linear Regression, it is considered the most suitable model for this problem.

## Key Dependencies
- Python 3.x
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- TensorFlow/Keras (for ANN)
- Word2Vec (Gensim library)
- Google Colab (for Google Drive integration)

## How to Run the Project
1. Clone this repository and navigate to the project directory.
2. Ensure you have the required dependencies installed.
