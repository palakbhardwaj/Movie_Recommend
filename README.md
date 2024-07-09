# 🎬 Movie Recommender System 🎬

Unlock a world of cinematic wonders with our state-of-the-art Movie Recommender System! By leveraging cutting-edge TF-IDF vectorization and cosine similarity, we bring you personalized movie suggestions that resonate with your taste.

## 📚 Table of Contents
- [✨ Overview](#-overview)
- [🚀 Features](#-features)
- [🛠️ Installation](#%EF%B8%8F-installation)
- [🎯 Usage](#-usage)
- [🎞️ Dataset](#-dataset)
- [🔍 Methodology](#-methodology)
  - [🧮 TF-IDF Vectorization](#-tf-idf-vectorization)
  - [📐 Cosine Similarity](#-cosine-similarity)
- [🔧 Example](#-example)
- [🤝 Contributing](#-contributing)
- [📜 License](#-license)

## ✨ Overview
Immerse yourself in a seamless movie discovery experience. Our system analyzes movie plots to recommend films that align with your preferences.

## 🚀 Features
- **TF-IDF Vectorization:** Converts plot descriptions into meaningful numerical vectors.
- **Cosine Similarity:** Measures the similarity between movies based on their vectorized plots.
- **Interactive Interface:** Input your favorite movie and receive a curated list of recommendations.

## 🛠️ Installation
To get started with our Movie Recommender System, follow these simple steps:

1. **Clone the repository:**
    ```sh
    git clone https://github.com/yourusername/movie-recommender-system.git
    cd movie-recommender-system
    ```

2. **Install the required packages:**
    ```sh
    pip install -r requirements.txt
    ```

## 🎯 Usage
1. Ensure you have the dataset file `movies.csv` in the root directory.

2. Run the recommendation script:
    ```sh
    python recommend.py
    ```

3. Enter the name of your favorite movie when prompted and receive your recommendations!

## 🎞️ Dataset
The dataset should be a CSV file with the following columns:
- `index`: Unique identifier for each movie.
- `title`: The title of the movie.
- `overview`: The plot description of the movie.
- and much more

## 🔍 Methodology
### 🧮 TF-IDF Vectorization
TF-IDF (Term Frequency-Inverse Document Frequency) transforms text data into numerical vectors, highlighting the importance of words in each plot relative to the entire dataset.

### 📐 Cosine Similarity
Cosine similarity measures the cosine of the angle between two vectors, providing a metric for movie similarity. It's particularly effective for text-based recommendations.

The formula for cosine similarity is:

\[ \text{cosine similarity} = \frac{\vec{A} \cdot \vec{B}}{\|\vec{A}\| \|\vec{B}\|} \]

Where:
- \(\vec{A}\) and \(\vec{B}\) are the TF-IDF vectors of two movies.
- \(\cdot\) represents the dot product of the vectors.
- \(\|\vec{A}\|\) and \(\|\vec{B}\|\) are the magnitudes of the vectors.

## 🔧 Example
Here's a quick example of how the recommendation system works:

1. **User Input:** "Inception"
2. **System Process:**
    - Vectorize the plot descriptions using TF-IDF.
    - Compute the cosine similarity between "Inception" and all other movies.
    - Sort the movies based on similarity scores.
3. **Output:** A curated list of movies similar to "Inception".

