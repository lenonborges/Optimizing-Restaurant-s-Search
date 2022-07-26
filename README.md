# Optimizing the Restaurant Search

Summary
-Introduction

-Business Problem

-Data to solve the problem

-Results

-Discussion

-Conclusion

Introduction
This project's goal is to deliver the n best food venues (considering the best quality x price relation) near you. We will get the data for some food venues places in Rio de Janeiro since the Foursquare API limits the response objects.

As human beings we tend to get annoyed of going to the same places over and over, so it would be nice if we got a list of the n best options in a price vs quality view. Then we can choose amongst a list which best suit for us on that particular moment.

Business Problem
Nowadays, on May 2021, Google maps allows filter for price and quality given a particular area on the map. It also gives you a list of places with filter for quality levels in steps of 0.5 points of difference. Although, Google maps already has great filters such as: Romantic, Cozy, Fun and others. However there is no filter for a good and not expensive place to go.

Therefore, the audience of this project is every person who wants to get a new, good and affordable place to eat.

Data to solve the problem
We'll use the Foursquare API to gather data for venues in a given City. The data is such as location, latitude, longitude, name, price, rating and others.

With these data we will construct a factor given weights for price and rating, actually 30% for price and 70% for rating. Where price has a negative effect and rating has a positive effect on our factor.

We will also use the Follium library to plot that found venues on map.
