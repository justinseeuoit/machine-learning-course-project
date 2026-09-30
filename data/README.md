## Music Genre and Emotion Dataset

Dataset Link: https://www.kaggle.com/datasets/colabsss/multimodal-music-genre-and-emotion-dataset

Dataset License: CC0: Public Domain

This dataset includes five thousand different songs, each with several features ascribed to them. These features describe the song's genre, tempo, energy, danceability, loudness, acousticness, instrumentalness, and valence, with these being used to predict a target variable of emotion. Each entry also has an ID associated with it, which is redundant for prediction purposes as each song has a unique ID. With the exception of genre, all of these features are continuous double values, and there are several different discrete values for the target. This could make classification more challenging, especially if one or more target clusters lack clear separation from its neighbors.

This dataset required very little cleaning, as there were no columns with missing or corrupted data that needed to be corrected. In the loudness column, some values read -0.0 instead of 0.0, which were normalized. Before proceeding to Phase 3, the dataset will be pruned of the Track_ID column since it is completely useless for prediction purposes and pandas already has native row IDs for dataframes. A second copy of the dataset will also be created, lacking the Emotion_Label column, as this target variable will need to be excluded from training and testing, while keeping a copy with said value intact for measuring accuracy, precision, and entropy.