What is it

A simple movie recommender made in python and jupyter notebook using Surprise, a python scikit for building recommender systems. The dataset that was used is the Movie lens movies dataset. 

How it works

The  python has a function which takes the name of a movie and the user ID (taken from the dataset) and uses Collaborative Filtering, with the help of Singular Vector Decomposition (SVD), to find which movies should be suggested. The theory behind Collaborative Filtering is that if group of users similar to a certain user like a certain thing then that user must also like that thing. SVD will be used to minimise the root mean square error and give better recommendations. The surprise library gives access to these methods very easily and thats the reason it was used. 

When the name of the movie is passed along with the user ID, the method will find the movie ID, and pass it into the SVD.predict method in order to predict the estimated rating that the user might give it. In this case it's on a scale of 5 and hence the higher the rating the more likey the user will like the movie. 

Links Referenced:
https://grouplens.org/datasets/movielens/latest/
https://www.kaggle.com/rounakbanik/movie-recommender-systems