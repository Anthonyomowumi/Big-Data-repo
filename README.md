# APPLICATION OF FP GROWTH ALGORITHM IN THE RECOMMENDATION OF NEW ARTISTS FOR USER

## I. Project Summary
This research was done to recommend/forecast which artist labels people are interested in, by analyzing trends in the listening behaviors of radio listeners’ datasets using FP Growth, one pf Association mining algorithms

## II. Dataset Description
The domain of the dataset is related to music. The lastfm dataset used for the study has 289955 records across 4 columns (user, artist, sex, and country). The lastfm dataset was examined using a common data mining and modeling methodology. 

## III. Methodology
The methodology for this project involved applying four techniques within the big data analytics lifecycle. These techniques include: 
##### 1.) Data Preprocessing and Validation 2.) Exploratory Analysis 3.) Data Visualization 4.) Association Rule Mining using FP Growth Algorithm 

Pyspark, a python API for spark was used to read and analyze the dataset in Google Collab programmatically. Also, the Pandas’ library was used to create a data frame (table-like) format that makes it simple to apply Matplotlib, Seaborn, and Plotly on the dataset for data visualization while , the Frequent Pattern Growth Algorithm was employed to identify the dataset's frequently occurring patterns.

### 1. Data Preprocessing and Validation: 
The major cleaning done on the dataset under data preprocessing was to drop the duplicates in the dataset using the dropDuplicates() command which after being done, the number of rows reduced to 289953 while the data was validated for missing and noisy dataset which none was found.

### 2. Exploratory Analysis and Data Visualization: 
The Pandas’ library was used to create a data frame (table-like) format that makes it simple to apply Matplotlib, Seaborn, and Plotly on the dataset for data visualization
