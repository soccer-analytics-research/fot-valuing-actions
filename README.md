# Friends of Tracking: Valuing actions in football

This repository provides presentations and tutorials that demonstrate how to value on-the-ball actions in football.

The tutorials use the open-source [socceraction](https://github.com/ML-KULeuven/socceraction) Python library and the publicly available [Wyscout match event dataset](https://figshare.com/collections/Soccer_match_event_dataset/4415000).

The dataset includes data for the 2017/2018 English Premier League, the 2017/2018 Spanish Primera División, the 2017/2018 German 1. Bundesliga, the 2017/2018 Italian Serie A, the 2017/2018 French Ligue 1, the 2018 FIFA World Cup and the UEFA Euro 2016. The dataset covers 1,941 matches, 3,251,294 events and 4,299 players.

The [environment.yml](environment.yml) file and [requirements.txt](requirements.txt) file list the required Python dependencies. The notebooks are compatible with version `0.2.0` of the `socceraction` Python library. If a more recent version of the library is installed, the code may need to be adapted.


## Content
### Introduction in Friends of Tracking ([video](https://www.youtube.com/watch?v=w0LX-2UgyXU))
This introductory presentation, which was given in the [Friends of Tracking](https://www.youtube.com/channel/UCUBFJYcag8j2rm_9HkrrA7w) session that took place on Thursday 7 May 2020, motivates the use of data for player recruitment in football, shows the limitations of traditional statistics to assess the performances of football players, introduces a number of frameworks for valuing actions of football players, provides an intuitive explanation of the VAEP framework for valuing actions of football players, and introduces the content of this series of hands-on video tutorials.

### Presentation: Valuing actions in football ([video](https://www.youtube.com/watch?v=xyyZLs_N1F0), [slides](https://drive.google.com/open?id=1t-jPgQFjZ7K4HRduaZWexUOMOmc1XR9H1jVWwaZYsOU))
This presentation expands on the content of the introductory presentation by discussing the technicalities behind the VAEP framework for valuing actions of football players as well as the content of the hands-on video tutorials in more depth.

### Tutorial 1: Run pipeline ([video](https://www.youtube.com/watch?v=0ol_eLLEQ64), [notebook](notebooks/tutorial1-run-pipeline.ipynb), [notebook on Google Colab](https://colab.research.google.com/github/SciSports-Labs/fot-valuing-actions/blob/master/notebooks/tutorial1-run-pipeline.ipynb))
This tutorial demonstrates the entire pipeline of ingesting the raw Wyscout match event data to producing ratings for football players. This tutorial touches upon the following four topics: downloading and preprocessing the data, valuing game states, valuing actions and rating players.

### Tutorial 2: Generate features ([video](https://www.youtube.com/watch?v=Ep9wXQgAFaE), [notebook](notebooks/tutorial2-generate-features.ipynb), [notebook on Google Colab](https://colab.research.google.com/github/SciSports-Labs/fot-valuing-actions/blob/master/notebooks/tutorial2-generate-features.ipynb))
This tutorial demonstrates the process of generating features and labels. This tutorial touches upon the following three topics: exploring the data in the SPADL representation, constructing features to represent actions and constructing features to represent game states.

### Tutorial 3: Learn models ([video](https://www.youtube.com/watch?v=WlORqYIb-Gg), [notebook](notebooks/tutorial3-learn-models.ipynb), [notebook on Google Colab](https://colab.research.google.com/github/SciSports-Labs/fot-valuing-actions/blob/master/notebooks/tutorial3-learn-models.ipynb))
This tutorial demonstrates the process of splitting the dataset into a training set and a test set, learning baseline models using conservative hyperparameters for the learning algorithm, optimizing the hyperparameters for the learning algorithm and learning the final models.

### Tutorial 4: Analyze models and results ([video](https://www.youtube.com/watch?v=w9G0z3eGCj8), [notebook](notebooks/tutorial4-analyze-models-and-results.ipynb), [notebook on Google Colab](https://colab.research.google.com/github/SciSports-Labs/fot-valuing-actions/blob/master/notebooks/tutorial4-analyze-models-and-results.ipynb))
This tutorial demonstrates the process of analyzing the importance of the features that are included in the trained machine learning models, analyzing the predictions for specific game states, and analyzing the resulting player ratings.


## References
* Tom Decroos, Lotte Bransen, Jan Van Haaren, and Jesse Davis. [Actions Speak Louder than Goals: Valuing Player Actions in Soccer.](https://arxiv.org/abs/1802.07127) In *Proceedings of the 25th ACM SIGKDD International Conference on Knowledge Discovery & Data Mining*, pp. 1851-1861. 2019.
* Luca Pappalardo, Paolo Cintia, Alessio Rossi, Emanuele Massucco, Paolo Ferragina, Dino Pedreschi, and Fosca Giannotti. [A Public Data Set of Spatio-Temporal Match Events in Soccer Competitions.](https://www.nature.com/articles/s41597-019-0247-7) *Scientific Data 6*, no. 1 (2019): 1-15.


## Authors
* [Lotte Bransen](http://www.twitter.com/LotteBransen)
* [Jan Van Haaren](http://www.twitter.com/JanVanHaaren)
