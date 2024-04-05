# ⛵ Usage ⛵

**Required packages**

To run this project, if you don't already have the required packages installed, then run:

```
pip install -r requirements.txt
```

**Information about the data**

Since the data files utilized in this project are too large to commit, I have only commited the [cleaned and merged dataset](../data/preprocessed/music_data.csv) created after running [dataCleaning.ipynb](./dataCleaning.ipynb). If entire dataset is required for evaluation, please reach out to me for details.

This is the original structure of the data subdirectory:

```
├── data
│   ├── preprocessed
│   │   ├── audio_info.csv (not uploaded)
│   │   ├── music_data.csv (uploaded on github)
│   │   └── tracks_info.csv (not uploaded)
│   └── raw
│       ├── echonest.csv (not uploaded)
│       ├── genres.csv (not uploaded)
│       └── tracks.csv (not uploaded)
```
