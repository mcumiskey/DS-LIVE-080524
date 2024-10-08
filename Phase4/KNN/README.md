# K-Nearest Neighbors

## Learning Goals

- describe the k-nearest neighbors algorithm
- identify multiple common distance metrics
- tune k appropriately in response to models with high bias or variance

## Lecture Materials

[Jupyter Notebook: KNN](knn.ipynb)

## Lesson Plan

### Introduction (5 Mins)

Basic idea here of making predictions based on known values of similar points. k-NN can be used for both regression and classification problems. The classification-version is more intuitive and will be explored here.

### Illustration on iris Dataset 10 Mins)

The code shows species predictions for a collection of nine irises, where the plots will illustrate the nearest neighbors for each plant. Notes:

- This is a three-nearest neighbors model
- The model uses only the first two columns from the iris dataset as predictors
- Some of the sets of three neighbors for the points we're predicting on include multiple species, hence the prediction probabilities will be values other than 1 and 0

### Deeper Analysis with titanic Dataset (20 Mins)

This section shows how the model performs on particular data points, accessing the indices from the DataFrame to keep track of them. Note that `NearestNeighbors().kneighbors()` re-indexes the data points starting at 0, and so we see these indices rather than the original DataFrame indices.

### Effects of Scaling (10 Mins)

Generally speaking we'll want to have some sort of scaling before fitting a k-NN model. (Otherwise we'll be comparing variables on different scales when making calculations of distance/similarity.)

### Bias/Variance and k (10 Mins)

Bias increases with k. This is perhaps easiest to see if you imagine increasing k all the way  up to n, the number of (training) data points. On such a model, all points would count as neighbors and so the model would simply predict the majority class every time.

### Conclusion (5 Mins)

There are alternatives when it comes to measuring distance. We'll say more about this in Phase 4 (clustering).