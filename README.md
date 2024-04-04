# APPLICATION OF FP GROWTH ALGORITHM IN THE RECOMMENDATION OF NEW ARTISTS FOR USER

## I. Project Summary
This research was done to recommend/forecast which artist labels people are interested in, by analyzing trends in the listening behaviors of radio listeners’ datasets using FP Growth, one pf Association mining algorithms

## II. Dataset Description
The domain of the dataset is related to music. The lastfm dataset used for the study has 289955 records across 4 columns (user, artist, sex, and country). The lastfm dataset was examined using a common data mining and modeling methodology. 

## III. Methodology
The methodology for this project involved applying four techniques within the big data analytics lifecycle. These techniques include: 
##### 1.) Data Preprocessing and Validation 2.) Exploratory Analysis & Data Visualization 3.) Association Rule Mining using FP Growth Algorithm 

The outlined methodology was executed programmatically on the Google Colab platform using PySpark, the Python API for the Apache Spark framework. PySpark was chosen for its adeptness in managing big data mining tasks, owing to its flexibility, scalability, and rapid execution.

while , the Frequent Pattern Growth Algorithm was employed to identify the dataset's frequently occurring patterns.

### 1. Data Preprocessing and Validation: 
The major cleaning done on the dataset under data preprocessing was to drop the duplicates in the dataset using the dropDuplicates() command which after being done, the number of rows reduced to 289953 while the data was validated for missing and noisy dataset which none was found.

### 2. Exploratory Analysis and Data Visualization: 
Numeric transformations, such as country-wise and artist-wise distribution, as well as calculating averages by country and sex, along with user distribution, were conducted on the dataframe utilizing the groupby method. These transformations were visually depicted through bar charts using the visualization libraries provided by Pandas, namely Matplotlib and Seaborn.

### 3. Association Rule Mining using FP Growth
The frequent itemset mining analysis is implemented using the FP-Growth machine learning algorithm with weights of 70% train data and 30% test data yielding 10534 for model training and 4466 for testing the model's performance. the dataset was first grouped to include every artist a user is currently listening to. Frequent pattern mining aims to find all the “interesting rules” that minimum support and confidence threshold that give all possible associations among the frequent music artists.  For frequent item mining and association rule generation, 3 hyperparameter tuning was done to get the optimal minSupport (S) and minConfidence (C) that will best suit for training the model which will aid maximize the model’s predictive accuracy (To evaluate which model has the best music recommendation performance)

## IV. Recommendation Results/Conclusion
3 hyperparameter tuning was done and finally the first was taken because it yielded the highest and optimal lift of 14.25207 from a combination of the antecedent and consequent. The frequent itemset count of the first hyperparameter yielded 1688 and an association rule count of 487 respectively. However, employing other unsupervised Association rule mining algorithms on the dataset is recommended for comparison; this will allow the best algorithms to be chosen for recommending artists to each unique user in the dataset.
