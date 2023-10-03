# Codeclause Internship : Project 2
# Movie Recommendation System

![download%20%281%29.png](attachment:download%20%281%29.png)

## How to Build a Movie Recommendation System

Have you ever wondered how YouTube recommends content, or how Facebook recommends you, new friends? Perhaps you’ve noticed similar recommendations with LinkedIn connections, or how Amazon will recommend similar products while you’re browsing. All of these recommendations are made possible by the implementation of recommender systems.

Recommender systems encompass a class of techniques and algorithms that can suggest “relevant” items to users. They predict future behavior based on past data through a multitude of techniques including matrix factorization.

In this article, I’ll look at why we need recommender systems and the different types of users online. Then, I’ll show you how to build your own movie recommendation system using an open-source dataset.

## Why Do We Need Recommender Systems?

We now live in what some call the “era of abundance”. For any given product, there are sometimes thousands of options to choose from. Think of the examples above: streaming videos, social networking, online shopping; the list goes on. Recommender systems help to personalize a platform and help the user find something they like.

The easiest and simplest way to do this is to recommend the most popular items. However, to really enhance the user experience through personalized recommendations, we need dedicated recommender systems.

From a business standpoint, the more relevant products a user finds on the platform, the higher their engagement. This often results in increased revenue for the platform itself. Various sources say that as much as 35–40% of tech giants’ revenue comes from recommendations alone.

Now that we understand the importance of recommender systems, let’s have a look at types of recommendation systems, then build our own with open-sourced data!

## Types of Recommender Systems

Machine learning algorithms in recommender systems typically fit into two categories:

- content-based systems and
- collaborative filtering systems.
- Modern recommender systems combine both approaches.
Let’s have a look at how they work using movie recommendation systems as a base.

## A) Content-Based Movie Recommendation Systems

Content-based methods are based on the similarity of movie attributes. Using this type of recommender system, if a user watches one movie, similar movies are recommended. For example, if a user watches a comedy movie starring Adam Sandler, the system will recommend them movies in the same genre or starring the same actor, or both. With this in mind, the input for building a content-based recommender system is movie attributes.

![download%20%282%29.png](attachment:download%20%282%29.png)

## B) Collaborative Filtering Movie Recommendation Systems

With collaborative filtering, the system is based on past interactions between users and movies. With this in mind, the input for a collaborative filtering system is made up of past data of user interactions with the movies they watch.

For example, if user A watches M1, M2, and M3, and user B watches M1, M3, M4, we recommend M1 and M3 to a similar user C. You can see how this looks in the figure below for clearer reference.

![download%20%283%29.png](attachment:download%20%283%29.png)

This data is stored in a matrix called the user-movie interactions matrix, where the rows are the users and the columns are the movies.

Now, let’s implement our own movie recommendation system using the concepts discussed above.

## The Dataset
For our own system, we’ll use the open-source TMDB 5000 Movie Dataset dataset from GroupLens. This dataset contains 100K data points of various movies and users.
link - https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata/data
