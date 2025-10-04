# Movie Recommendation System

This repository contains a Movie Recommendation System built using Python and pandas. The main goal of this project is to process and analyze a movie dataset to extract relevant features and build a foundation for recommending movies based on genres, keywords, cast, and crew information.

## Features

- Loads and merges movie metadata and credits from the TMDB 5000 Dataset.
- Cleans and preprocesses data (handles missing values and duplicates).
- Extracts relevant features such as genres, keywords, top 3 cast members, and director.
- Prepares data for further feature engineering and similarity-based recommendations (e.g., content-based filtering).

## Dataset

The project uses the [TMDB 5000 Movie Dataset](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata) which contains two CSV files:
- `tmdb_5000_movies.csv`
- `tmdb_5000_credits.csv`

These files should be present in the same directory as the notebook.

## Project Workflow

1. **Import Libraries**: Uses `numpy`, `pandas`, and `ast` for data processing.
2. **Load Data**: Reads the movies and credits datasets.
3. **Inspect Data**: Displays sample rows from both datasets for understanding structure.
4. **Merge Data**: Merges movies and credits datasets on the `title` column.
5. **Select Features**: Keeps only important columns for recommendation.
6. **Data Cleaning**: Drops nulls and removes duplicates.
7. **Feature Extraction**: 
    - Parses genres and keywords into lists.
    - Extracts top 3 cast members.
    - (Further steps may include extracting directors and building recommendation logic.)
8. **Prepare for Recommendation**: Data is now ready for feature engineering and building recommendation algorithms.

## How to Run

1. Clone this repository:
    ```bash
    git clone https://github.com/shiblesadik603/MovieRecommandarSystem.git
    cd MovieRecommandarSystem
    ```
2. Download the [TMDB 5000 Movie Dataset](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata) and place the CSV files in the root directory.
3. Open `MovieRecommanderSystem.ipynb` using Jupyter Notebook or JupyterLab.
4. Run the cells step by step to preprocess the data.

## Requirements

- Python 3.x
- pandas
- numpy
- Jupyter Notebook or JupyterLab

Install dependencies using:
```bash
pip install pandas numpy jupyter
```

## Example Usage

The notebook demonstrates:
- How to merge and process movie metadata.
- How to extract lists of genres, keywords, and key cast members.
- How to clean and prepare the data for recommendations.

You can extend this notebook to build a content-based or collaborative filtering recommendation engine.

## Acknowledgements

- [TMDB 5000 Dataset](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata) on Kaggle
- pandas and numpy libraries

## License

This project is for educational purposes.

---
*Created by shiblesadik603*
