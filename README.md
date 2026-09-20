# Spotify Dataset Analysis: Music Popularity, Recommendations & Clustering

## Overview

This project explores a Spotify music dataset to investigate the relationship between audio features and song popularity, develop a content-based song recommendation system, and identify natural groupings within songs using unsupervised learning techniques.

The project combines **data analysis, machine learning, and data visualisation** to transform raw music data into meaningful insights about listener preferences and musical characteristics.

## Objectives

The project was designed around three main objectives:

* Identify audio features that are associated with song popularity.
* Develop a recommendation system that can identify songs with similar characteristics.
* Explore patterns and groupings within songs using clustering techniques.

## Dataset

The dataset contains information about songs and their audio characteristics, including features such as:

* Danceability
* Energy
* Loudness
* Acousticness
* Instrumentalness
* Liveness
* Valence
* Speechiness
* Tempo
* Song popularity

These features provide quantitative measures that can be used to explore relationships between the characteristics of a song and its popularity.

## Methodology

### 1. Data Exploration and Preprocessing

The dataset was first explored and prepared for analysis. This included examining the structure of the data, identifying relevant variables, and preparing the audio features for machine-learning analysis.

### 2. Song Popularity Prediction

A **Random Forest classifier** was used to investigate which audio features were most influential in predicting song popularity.

The analysis identified:

* **Loudness**
* **Acousticness**
* **Danceability**

as some of the most influential features in the model.

The results suggested that popular songs in the dataset tended to be louder, less acoustic, and more rhythmically engaging.

### 3. Song Recommendation System

A **k-Nearest Neighbors (kNN)** approach was used to identify songs with similar audio characteristics.

The system used **cosine similarity** to compare songs based on their feature representations and retrieve songs with similar characteristics to a given input track.

This demonstrated how content-based recommendation systems can be developed using audio features, without relying solely on user interaction data.

### 4. Clustering Analysis

Unsupervised learning was used to explore whether songs naturally formed groups based on their audio characteristics.

The analysis identified two primary clusters:

* **Cluster 0:** Softer, more acoustic and lower-energy songs.
* **Cluster 1:** Louder, higher-energy songs that were more characteristic of mainstream/popular styles.

These clusters demonstrated how quantitative audio characteristics can reveal patterns and similarities between songs without relying on predefined genre labels.

## Key Findings

The analysis produced several notable findings:

1. **Audio characteristics can provide useful information about song popularity.**
   Loudness, acousticness, and danceability were among the most influential variables in predicting popularity.

2. **Content-based recommendation is feasible using audio features.**
   The kNN model was able to identify songs with similar characteristics using cosine similarity.

3. **Unsupervised learning can reveal meaningful patterns.**
   Clustering identified groups of songs with different levels of energy, acousticness, and intensity.

4. **Quantitative data can provide insights into subjective experiences.**
   Although music is highly personal and cultural, measurable characteristics can still be used to identify patterns in listener preferences and musical structure.

## Recommendations

Based on the findings, several potential applications were identified:

### For Streaming Platforms

Audio-feature-based recommendation systems could complement collaborative filtering approaches, particularly for new or less-known songs with limited user interaction data.

### For Artists and Producers

Understanding the characteristics associated with popularity could provide additional data-driven insights when developing music for particular audiences.

### For Music Analysts and Researchers

Future analyses could combine audio features with additional information such as lyrics, genre, release year, mood, and listener behaviour to develop a more comprehensive understanding of musical trends.

## Limitations

The analysis has several limitations:

* It focuses primarily on audio features and does not account for lyrics or contextual information.
* Listener demographics and individual preferences were not included.
* Social factors influencing popularity were not considered.
* The clustering analysis focused on two groups, which may not capture the full complexity of musical genres and styles.
* Popularity is influenced by many factors beyond the measurable characteristics of a song.

## Future Work

Potential extensions of this project include:

* Incorporating **time-series analysis** to examine how musical characteristics and popularity change over time.
* Including **listener behaviour**, such as skips, replays, and listening frequency.
* Incorporating **lyrics and natural language processing** into the analysis.
* Exploring additional clustering techniques such as hierarchical clustering and DBSCAN.
* Developing a more advanced recommendation system combining audio features with user behaviour.
* Experimenting with deep-learning approaches for more complex pattern recognition.
* Building an interactive dashboard to allow users to explore the dataset and findings.

## Technologies Used

* **Python**
* **Pandas** – Data manipulation and analysis
* **NumPy** – Numerical computing
* **Matplotlib / Seaborn** – Data visualisation
* **Scikit-learn** – Machine learning, classification, clustering and similarity analysis
* **Jupyter Notebook** – Data analysis and experimentation

## Project Structure


spotify-dataset-analysis/
│
├── spotify_dataset.csv
│
├── spotify_analysis.ipynb
│
├── preprocessed_dataset.csv
│
│
└── README.md
``



## Conclusion

This project demonstrates how machine-learning and quantitative analysis can be applied to a real-world dataset to uncover patterns, generate recommendations, and support data-driven decision-making.

By combining supervised learning, recommendation techniques, and unsupervised clustering, the project provides a practical example of how raw data can be transformed into meaningful insights and potential applications.

## Author

Michelle Naa Kwarley Owoo

