# Music Recommendation System Using Clustering Analysis

## Abstract

This data science project explores the application of clustering techniques to develop a simple, personalized music recommendation system that uses audio trats to compare songs. By analyzing musical features and patterns, we aim to create meaningful groupings of similar songs that can enhance recommendation accuracy and user experience.

## 1. Introduction

### 1.1 Problem Statement
Traditional music recommendation systems often struggle with the "cold start" problem and can create echo chambers of similar recommendations. This project addresses these limitations by implementing an unsupervised learning approach using clustering techniques to identify natural groupings in music data.

### 1.2 Objectives
- Develop a clustering-based recommendation system for music
- Identify meaningful patterns in musical features
- Create an interpretable model for song similarity

## 2. Methodology

### 2.1 Data Collection
The project utilizes music feature data including:
- Audio characteristics (tempo, duration, energy, etc.)
- Genre classifications (assisting the audio traits in gaining more well defined clusters)
- User interaction

### 2.2 Data Preprocessing
- Handling missing values
- Feature engineering
- Feature scaling and normalization
- Dimensionality reduction techniques

### 2.3 Clustering Analysis
Implementation of clustering algorithms to group similar songs based on their features. The analysis includes:
- KMeans Algorithm selection
- Parameter tuning
- Cluster evaluation metrics
- Visualization of results

## 3. Implementation

The complete analysis and implementation can be found in `final_notebook.ipynb`, which contains:
- Detailed data exploration
- Feature preprocessing steps
- Clustering model implementation
- Visualization of results
- Recommendation generation logic

### Project Structure
```
.
├── data/               # Raw dataset
├── images/            # Generated visualizations
├── final_notebook.ipynb # Main analysis notebook
└── README.md          # Project documentation
```

## 4. Results and Discussion

### 4.1 Key Findings
- Identification of 2 somewhat distinct music clusters, however, the amount of songs and genres makes it hard to qualify them as accurate and reliable for narrowing down similar songs.
- Additional help from genre (an already substantial method of dividing and recommending similar songs) to add weight to the recommendations to help narrow down groups of songs outside of purely audio traits.
- The recommendation is simple and grabs a handful of songs that have similar traits and genre.
- With the overlay of subgenre and genre over the clusters, we can see that even within the genres there can be a very wide stetch and variety of characteristics so recommending purely based on these features proves difficult because it doesnt take into consideration a users overall music preferences (instruments, lyrics, overall emotional aspect).

### 4.2 Visualizations
The `images/` directory contains visualizations including:
- Cluster distributions
- Feature importance plots
- Performance metrics

### 4.3 Limitations and Future Work
- With the overlay of subgenre and genre over the clusters, we can see that even within the genres there can be a very wide stetch and variety of characteristics so recommending purely based on these features proves difficult because it doesnt take into consideration a users overall music preferences (instruments, lyrics, overall emotional aspect).
- Potential improvements include adding back in more features such as mode, key, and potentially lyrics embedding for emotional context might improve performance.

## 5. Technical Requirements

### Environment Setup
```bash
Python 3.x
Jupyter Notebook
Required libraries: numpy, pandas, scikit-learn, matplotlib, seaborn
```

### Running the Analysis
1. Clone the repository
2. Install dependencies
3. Open and run `final_notebook.ipynb`

## 6. References

- Data sources : Kaggle https://www.kaggle.com/datasets/imuhammad/audio-features-and-lyrics-of-spotify-songs/data 

## 7. Contributors

Project developed as part of data science research/coursework.

---
*Note: For detailed implementation and results, please refer to the Jupyter notebook in this repository.*