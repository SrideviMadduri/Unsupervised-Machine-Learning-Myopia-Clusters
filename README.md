# Unsupervised Machine Learning Myopia-Clusters

The purpose of the assignment was used to process the raw MYOPIA data to fit the machine learning models. Several clustering algorithms were used to explore if the patients can be placed into distinct groups of patients. This would help us to analyze them separately and to find better ways to predict myopia, or nearsightedness.

## Part 1: Prepare the Data
Used Pandas DataFrame to read myopia.csv.

Removed the "MYOPIC" column from the dataset.

Verified if the data has any "Nulls" or duplicates

Standardize the dataset (using StandardScaler) so that columns that contain larger values do not influence the outcome more than columns with smaller values.

## Part 2: Apply Dimensionality Reduction
Performed dimensionality reduction with PCA. This reduced the number of columns from 14 to 10 features.

preserved 90% of the explained variance in dimensionality reduction.
Further reduced the dataset dimensions with t-SNE.

Created a scatter plot of the t-SNE output. Looks like there are 5 distinct clusters.


scatterPlot

![alt text](https://github.com/SrideviMadduri/unsupervised-machine-learning-challenge/blob/main/Images/download%20(1).png)



## Part 3: Perform a Cluster Analysis with K-means
Created an elbow plot to identify the best number of clusters.

Used a for loop to determine the inertia for each k between 1 through 10.

Determined where the elbow of the plot is, and at which value of k it appears.

elbowCurve

![alt text](https://github.com/SrideviMadduri/unsupervised-machine-learning-challenge/blob/main/Images/download.png)


## Part 4: Make a Recommendation
The elbow curve  shows that the patients can be grouped into 5 or 6 clusters. I would recommend to group the patients into 5 clusters because the elbow curve is more flat after 5 and we may be over fitting the data if we group the patients into 6 clusters.
