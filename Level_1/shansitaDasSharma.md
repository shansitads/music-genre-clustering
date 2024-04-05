# 🎻 Music Genre Clustering

> Level 1

### 📂 Dataset

FMA (Free Music Archive) Dataset: [website](https://freemusicarchive.org/) | [paper](https://arxiv.org/pdf/1612.01840.pdf) | [github](https://github.com/mdeff/fma/blob/master/baselines.ipynb)

The FMA dataset contains information about all the genres that a track can be categorized under, as well as information about the audio in itself.

### 📌 Focus Questions

Genre classification is a highly subjective process, changing on the basis of cultures and experience. My goal through this project is to identify how genres can be identified through a more quantitative process i.e. by clustering the tracks on the basis of the fundamental audio features of the track.
As defined by Spotify, the [essential features](https://help.spotontrack.com/article/what-do-the-audio-features-mean) that I have focused on are as follows:

1. Acousticness (confidence of the track being acoustic)
2. Danceability (tempo, rhythm stability, beat strength, and overall regularity)
3. Energy (intensity, dynamic range, perceived loudness, timbre, onset rate, and general entropy)
4. Instrumentalness
5. Liveness (presence of an audience)
6. Speechiness (presence of spoken words in a track)
7. Tempo (BPM)
8. Valence (musical positiveness or cheerfulness)

### 🧹 Dataset cleaning procedure

The general steps I followed to clean this dataset are

1. Fix data types
2. Fix indexing and multilevel indexing
3. Group subgenres into broader genres
4. Handle missing data: Data imputation / removal
5. Visualize data distributions
6. Merge all required and cleaned data into a single file and save it

### 🎁 Level 1 bonus tasks attempted:

- [x] using Python<br>
- [x] using a dataset that is not listed above<br>
- [x] using a dataset that is not from Kaggle<br>
- [x] coming up with your own focus question<br>
- [x] choosing a clustering problem<br>
- [x] choosing a Neural Network problem<br>
