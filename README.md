# Deep Learning for Nearest Neighbours & Regression on a Poster Dataset.
 Movie Poster dataset used to generate a Neural Network to find nearest neighbours and perform regression on their year of release, using Keras & Tensorflow

Code files:
1. 22222806_Assignment2.ipynb


# University of Galway
## CT5133 / CT5145 Deep Learning (/Online) 2022-2023
## Assignment 2
## James McDermott

In this assignment the goal is to take advantage of pre-trained NN models to create an embedding with a dataset of movie posters, and demonstrate how to use that embedding.

The dataset (`/DL_Sample`) is provided, along with some skeleton code for loading it.

The individual steps to be carried out are specified below, with `### YOUR CODE HERE` markers, together with the number of marks available for each part.

### Dataset Credits

The original csv file is from: 

https://www.kaggle.com/datasets/neha1703/movie-genre-from-its-poster

I have added the *year* column for convenience.

I believe most of the information is originally from the famous MovieLens dataset:

* https://grouplens.org/datasets/movielens/
* https://movielens.org/

However, I'm not clear whether the poster download URLs (Amazon AWS URLs) which are in the csv obtained from the Kaggle URL above are from a MovieLens source, or elsewhere.

To create the dataset we are using, I have randomly sampled a small proportion of the URLs in the csv, and downloaded the images. I have removed those which fail to download. Code below also filters out those which are in black and white, ie 1 channel only.
