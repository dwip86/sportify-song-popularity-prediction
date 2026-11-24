# Spotify Song Popularity Prediction 🎵

## Project Overview
This project uses machine learning to classify Spotify songs into popularity categories based on their audio features. It includes data exploration, preprocessing, model training, evaluation, comparison, and a sample new-song prediction.

## Popularity Categories
The notebook creates the target variable `popularity_category` from the song's `popularity` score:

- **Not Popular:** 0–39
- **Moderately Popular:** 40–69
- **Popular:** 70–100

## Dataset
Dataset file: `songs_normalize.csv`

The notebook uses these nine audio features:

- danceability
- energy
- loudness
- speechiness
- acousticness
- instrumentalness
- liveness
- valence
- tempo

The target column is `popularity_category`, derived from `popularity`.

## Machine Learning Models
1. Logistic Regression
2. Decision Tree Classifier
3. Random Forest Classifier

## Workflow
1. Import Python libraries and load the CSV dataset.
2. Inspect the dataset, summary statistics, missing values, and duplicates.
3. Remove duplicate rows.
4. Explore popularity and audio-feature distributions and correlations.
5. Create the three popularity categories.
6. Split the data into training and testing sets (80/20, stratified).
7. Scale features for Logistic Regression.
8. Train Logistic Regression, Decision Tree, and Random Forest models.
9. Evaluate models using accuracy, weighted precision, weighted recall, weighted F1-score, and classification reports.
10. Compare model performance and visualize the Random Forest confusion matrix and feature importance.
11. Predict the popularity category and class probabilities for a sample new song.

## Requirements
- Python 3
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- Jupyter Notebook (or Google Colab)

Install dependencies with:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

## How to Run
### Jupyter Notebook
1. Extract or open this project folder.
2. Start Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
3. Open `Spotify_Song_Popularity_Prediction.ipynb`.
4. Run the cells in order.
5. When prompted by the Google Colab upload cell, upload `songs_normalize.csv` if running in Colab. When running locally, the dataset should be in the notebook's working directory; replace the Colab-only upload cell with a normal local run if needed.

## Project Files
```text
Spotify-Song-Popularity-Prediction/
├── README.md
├── songs_normalize.csv
└── Spotify_Song_Popularity_Prediction.ipynb
```

## Author
**Abhijit Roy**
