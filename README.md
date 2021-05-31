# Spotify Recommendation Engine

[![forthebadge](https://forthebadge.com/images/badges/made-with-python.svg)](https://forthebadge.com)

![GitHub contributors](https://img.shields.io/github/contributors/pradyyadav/Spotify-Recommendation-Engine)    ![GitHub last commit](https://img.shields.io/github/last-commit/pradyyadav/Spotify-Recommendation-Engine)

![spotify](https://storage.googleapis.com/pr-newsroom-wp/1/2020/03/Header.png)

##### A content-based Recommendation system which recommends the songs a user may like. Based on user's previous interests, it uses clustering to find similar songs and finally recommend the most similar songs.

**Check this [notebook](https://drive.google.com/file/d/1nkmC-wGsGah02NBcEG9uVcbhe0R0uSpM/view?usp=sharing) for implementation**


## Table of contents
- [Introduction](https://github.com/pradyyadav/Spotify-Recommendation-Engine#Introduction)
- [About](https://github.com/pradyyadav/Spotify-Recommendation-Engine#About)
- [Technologies](https://github.com/pradyyadav/Spotify-Recommendation-Engine#Technologies)
- [Setup](https://github.com/pradyyadav/Spotify-Recommendation-Engine#Setup)

## Introduction
During the last few decades, with the rise of Youtube, Amazon, Netflix and many other such web services, recommender systems have taken more and more place in our lives. From e-commerce (suggest to buyers articles that could interest them) to online advertisement (suggest to users the right contents, matching their preferences), recommender systems are today unavoidable in our daily online journeys.

In a very general way, recommender systems are algorithms aimed at suggesting relevant items to users (items being movies to watch, text to read, products to buy or anything else depending on industries).

For a Recommendation system there are two most commonly used algorithms used by budding data scientists:
- ##### Content Based FIltering
    
    This technique is often used in recommender systems, which are algorithms designed to advertise or recommend things to users based on knowledge accumulated about the user.
- ##### Collaborative Filtering
    Collaborative filtering is a technique that can filter out items that a user might like on the basis of reactions by similar users.It works by searching a large group of people and finding a smaller set of users with tastes similar to a particular user. It looks at the items they like and combines them to create a ranked list of suggestions.

    ![concol](https://userscontent2.emaze.com/images/33a3dfc3-ee4e-4e6c-b5f0-35bf1635bc72/decf302dc639e1593fc56f205d074de1.png) 


#### Spotify
   
   <p align="center"><img src = "https://img.icons8.com/plasticine/2x/spotify.png"</p>

Digital cloud-based music platform that provides cross-device access to over 50 million songs, and a rapidly-rising number of podcasts. Founded in Stockholm in 2006. Spotify’s recommender system provides suggestions for users based on their historical interactions (listen/skip/add to playlist), the attributes of the songs/artists they listen to, and the preferences of what it deems “similar” users.

Well this repo demonstrates content-based recommendation, which categorises songs in form of clusters and then recommend the most similar songs.
## About
First of all, data of about 600,000 tracks are collected from [Spotify Dataset (1922-2021)](https://www.kaggle.com/yamaerenay/spotify-dataset-19212020-160k-tracks), each song consists of various features and based on these features, the songs are clustered using K-Means Clustering.
- #### K-means Clustering

    The objective of K-means is to group similar data points together and discover underlying patterns. To achieve this objective, K-means looks for a fixed number (k) of clusters in a dataset. A cluster refers to a collection of data points aggregated together because of certain similarities. Following is the plot depicting all the songs in clusters.
    
    ![cluster](https://github.com/pradyyadav/Images/blob/main/cluster.png?raw=true)
    
- #### Cosine Similarity 

    When recommending songs for a user's previous interests, the mean of all the features is used to centralised the predicting vector, then this centralised vector is then used for prediction and it forms a new data in the cluster it belongs, after the prediction it is necessary to find the most similar songs, thus cosine similarity helps to find the most relevant song in that cluster.
    
    ![cossim](https://datascience-enthusiast.com/figures/cosine_sim.png)
## Technologies

- #### Languages and Frameworks
- #### Libraries

## Setup
