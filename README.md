🎬 Movie Recommendation System

A Content-Based Movie Recommendation System built using Scikit-learn that suggests movies similar to a user’s favorite movie based on genres, keywords, tagline, cast, and director information.

📌 Overview

This project recommends movies by analyzing textual features of films and calculating similarity scores using TF-IDF Vectorization and Cosine Similarity.

The system takes a movie name as input and returns the top similar movies based on content similarity.

❓ Problem Statement

Users often struggle to discover new movies aligned with their interests. This system helps users find similar movies based on the content characteristics of a movie they already like.

🧠 Recommendation Approach

Type: Content-Based Filtering

The system:

Combines movie features (genre, keywords, tagline, cast, director)

Converts text data into numerical vectors using TF-IDF

Computes similarity using Cosine Similarity

Suggests top similar movies

📂 Dataset

Dataset Source:
YBI Foundation Movie Recommendation Dataset

The dataset includes:

Movie_Title

Movie_Genre

Movie_Keywords

Movie_Tagline

Movie_Cast

Movie_Director

Movie_ID

⚙️ Tech Stack

Python

Pandas

NumPy

Scikit-learn

Difflib

🛠️ How It Works
1️⃣ Data Preprocessing

Load dataset

Select relevant features

Handle missing values

Combine textual features

2️⃣ Feature Engineering

Convert text data into numerical vectors using:

TfidfVectorizer

3️⃣ Similarity Computation

Compute similarity matrix using:

cosine_similarity

4️⃣ Movie Matching

Use difflib.get_close_matches() to handle approximate movie name input

5️⃣ Recommendation

Sort movies based on similarity score

Display top 30 similar movies

▶️ How to Run the Project
Step 1: Clone the Repository
git clone https://github.com/your-username/movie-recommendation-system.git
cd movie-recommendation-system
Step 2: Install Required Libraries
pip install pandas numpy scikit-learn
Step 3: Run the Notebook

Open the Jupyter Notebook:

jupyter notebook

Run all cells and enter your favorite movie name when prompted:

Enter your favourite movie name:
📊 Example Output
Top 30 Movies Suggested for you:

1 - Movie Name A
2 - Movie Name B
3 - Movie Name C
...
🚀 Future Improvements

Add Collaborative Filtering

Build a Web Interface (Streamlit / Flask)

Deploy as a Web App

Add Movie Posters & Ratings

Optimize performance for large datasets

📁 Project Structure
MovieRecommendationSystem.ipynb
README.md
📜 License

This project is open-source and available under the MIT License.
