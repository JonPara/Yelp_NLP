## Yelp_NLP

In this project, I used NLP to classify Yelp Reviews into 1 to 5 star categories based off the context in the reviews.

Each observation in this dataset is a review of a particular business by a particular user.

The "stars" column is the number of stars (1 through 5) assigned by the reviewer to the business. (Higher stars is better.) In other words, it is the rating of the business by the person who wrote the review.

The "cool" column is the number of "cool" votes this review received from other Yelp users.

All reviews start with 0 "cool" votes, and there is no limit to how many "cool" votes a review can receive. In other words, it is a rating of the review itself, not a rating of the business. The "useful" and "funny" columns are similar to the "cool" column.

The Yelp Data Set came from Kaggle https://www.kaggle.com/c/yelp-recsys-2013


## Analysis

As seen below, we have a handful of data that we'll be working with for this particular project. 
![capture1](https://user-images.githubusercontent.com/33237727/42138611-32fda196-7d4e-11e8-9cb5-1c5a1ca800a2.JPG)



I created grids and plots to show a better visual representation that text length has a relationship with the amount of stars that it receives:
![capture2](https://user-images.githubusercontent.com/33237727/42138612-33097f0c-7d4e-11e8-8cb3-d861dddee289.JPG)
![capture3](https://user-images.githubusercontent.com/33237727/42138613-33147204-7d4e-11e8-90a0-d19017dbeed2.JPG)
![capture4](https://user-images.githubusercontent.com/33237727/42138614-331f41c0-7d4e-11e8-8621-eddb3a16f747.JPG)

Here's the beginning of my NLP classification task. I used several different scikit-learn libraries to obtain a prediction analysis on the model. 
![capture5](https://user-images.githubusercontent.com/33237727/42138615-332b9574-7d4e-11e8-8c19-fad6baf01aa9.JPG)
![capture6](https://user-images.githubusercontent.com/33237727/42138616-3336ac3e-7d4e-11e8-9b3c-c6b51974660b.JPG)

Later, I used Text Processing to evaluate the model:
![capture7](https://user-images.githubusercontent.com/33237727/42138617-3341e05e-7d4e-11e8-975f-9fb1d2c640ef.JPG)



In conclusion, tfidf did not work they we wanted to. The naive bayes model gave us a precision rate of 92% to see whether or not a rating of the review itself is not the rating of the business. 
