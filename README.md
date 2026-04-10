# CineSense - Intelligent Movie Recommendation System 🎬

CineSense is a modern, full-stack movie recommendation engine. It combines a fast API backend with a beautifully designed, responsive frontend to help you discover movies through intelligent search, content-based matching, and genre discovery.

## Features ✨

*   **Intelligent Search & Autocomplete**: Search for any movie and get instant suggestions powered by the TMDB API.
*   **Content-Based Recommendations**: Uses advanced NLP (TF-IDF vectorization and cosine similarity) on plot summaries, genres, and metadata to find movies similar to the ones you love.
*   **Genre Discovery**: Fallback and horizontal recommendations based on TMDB genre matching.
*   **Modern UI**: A sleek, responsive user interface built with Streamlit, featuring poster grids, movie details, and smooth navigation.
*   **High Performance**: Powered by a FastAPI backend with asynchronous routes and HTTPX for rapid external API calls.

## Tech Stack 🛠️

*   **Frontend**: Streamlit
*   **Backend**: FastAPI, Uvicorn
*   **Machine Learning**: Scikit-Learn (TF-IDF), Pandas, NumPy, SciPy
*   **External APIs**: TMDB (The Movie Database) API
*   **Other**: Python-dotenv, HTTPX

## Prerequisites 📋

1.  Python 3.9+ installed.
2.  A valid [TMDB API Key](https://developer.themoviedb.org/docs/getting-started).

## Installation & Setup 🚀

1.  **Clone the repository** (if you haven't already):
    ```bash
    https://github.com/kb-patel2005/movie_recommand_system_python.git
    ```

2.  **Create a Virtual Environment** (Recommended):
    ```bash
    python -m venv venv
    ```
`env/bin/activate`

3.  **Install Dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

## Running the Application ▶️

You need to run both the FastAPI backend and the Streamlit frontend.

**1. Start the FastAPI Backend:**
Open a terminal and run:
```bash
uvicorn main:app --reload
```

**2. Start the Streamlit Frontend:**
Open a **new** terminal, activate your virtual environment, and run:
```bash
streamlit run app.py
```

## Project Structure 📂

*   `app.py`: Streamlit frontend code.
*   `main.py`: FastAPI backend application and routes.
*   `movies.ipynb`: Jupyter notebook containing the data exploration and TF-IDF model training.
*   `df.pkl`, `indices.pkl`, `tfidf.pkl`, `tfidf_matrix.pkl`: Pre-computed machine learning models and data objects for fast recommendations.
*   `requirements.txt`: Python package dependencies.

## Acknowledgements 🙏
*   Data and imagery provided by [TMDB](https://www.themoviedb.org/).
