
# TMDB Movie Analysis

Exploratory data analysis of TMDB's top-rated movies using Python, Pandas, and the TMDB API.

## Overview

This project collects top-rated movie data from [The Movie Database (TMDB)](https://www.themoviedb.org/) and explores movie ratings, vote counts, and release-year trends using Python.

The goal is to practice API integration, data manipulation, data cleaning, and exploratory data analysis while extracting meaningful insights from real-world movie data.

## Objectives

- Retrieve movie data using the TMDB API.
- Store and manipulate data using Pandas DataFrames.
- Inspect data types, missing values, and duplicate records.
- Explore movie ratings, vote counts, and release dates.
- Identify trends and patterns in the collected dataset.
- Develop data visualizations to communicate findings.

## Tech Stack

- **Python** — Core programming language
- **Requests** — API requests and data retrieval
- **Pandas** — Data manipulation and analysis
- **Jupyter Notebook** — Interactive analysis
- **Matplotlib** — Data visualization (planned)

## Dataset

The data is collected from TMDB's Top Rated Movies API endpoint.

- **Source:** [TMDB Developer Documentation](https://developer.themoviedb.org/)
- **Records collected:** Up to 10,000 movies
- **Format:** JSON responses converted into a Pandas DataFrame

The dataset includes fields such as movie ID, title, overview, release date, average rating, and vote count.

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/tmdb-movie-analysis.git
cd tmdb-movie-analysis
```

### 2. Create a virtual environment

```bash
python -m venv .venv
```

Activate it on Windows PowerShell:

```powershell
.\.venv\Scripts\Activate.ps1
```

### 3. Install dependencies

```bash
pip install requests pandas python-dotenv matplotlib jupyter
```

### 4. Configure your API key

Obtain API access from [TMDB](https://developer.themoviedb.org/).

Create a `.env` file in the project root:

```env
API_KEY=your_actual_api_key
```

Load the key in Python:

```python
import os
from dotenv import load_dotenv

load_dotenv()
API_KEY = os.getenv("API_KEY")
```

**Important:** Never commit your `.env` file or expose your API key publicly.

### 5. Run the notebook

Open the project in VS Code, select your virtual environment as the Python kernel, and run `top_rated_movie.ipynb`.

## Analysis Performed

- Initial dataset inspection and summary statistics
- Missing-value checks
- Duplicate-record checks
- Highest-rated movies
- Movies with the highest vote counts
- Average movie rating
- Most frequent release years

Additional cleaning, visualizations, and insights will be developed as the project progresses.

## Project Structure

```text
tmdb-movie-analysis/
├── top_rated_movie.ipynb
├── .env                 # Local API key; not committed
├── .gitignore
└── README.md
```

## Future Improvements

- Complete data cleaning and validation
- Visualize rating and release-year distributions
- Investigate the relationship between ratings and vote counts
- Develop a more balanced movie-ranking approach
- Build an interactive movie-data dashboard
- Explore a movie recommendation system

## Acknowledgements

Movie data is provided by [The Movie Database (TMDB)](https://www.themoviedb.org/).

This project uses TMDB data but is not endorsed or certified by TMDB.

---

*Built as a hands-on project to strengthen Python, API integration, and data analysis skills.*
