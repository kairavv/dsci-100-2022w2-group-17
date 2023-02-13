# [Project Topic]
## Introduction
[Text]

    Provide some relevant background information on the topic so that someone unfamiliar with it will be prepared to understand the rest of your proposal
    Clearly state the question you will try to answer with your project
    Identify and describe the dataset that will be used to answer the question

## Methods
[Text]

    Explain how you will conduct either your data analysis and which variables/columns you will use. Note - you do not need to use all variables/columns       that exist in the raw data set. In fact, that's often not a good idea. For each variable think: is this a useful variable for prediction?
    Describe at least one way that you will visualize the results

### Preliminary exploratory data analysis

    Demonstrate that the dataset can be read from the web into R 
    Clean and wrangle your data into a tidy format
    Using only training data, summarize the data in at least one table (this is exploratory data analysis). An example of a useful table could be one that     reports the number of observations in each class, the means of the predictor variables you plan to use in your analysis and how many rows have missing     data. 
    Using only training data, visualize the data with at least one plot relevant to the analysis you plan to do (this is exploratory data analysis). An         example of a useful visualization could be one that compares the distributions of each of the predictor variables you plan to use in your analysis.


##### The preliminary exploratory data analysis will include:
- Reading dataset from web link
- Cleaning and wrangling data into a tidy format
- Splitting into training data and test data
- Summary statistics of training subset
- Visualization of training data predictors and determining appropriate predictors
```R
# load necessary libraries


# initialize custom color palette to accommodate for color blindness
COLOR_PALETTE <- c("#F8766D", "#CD9600", "#00BE67", "#00A9FF", "#8A7AFF", "#FF33FC") #Add more ig
```


#### Reading from web link
Read from link with appropriate delimiter.


```R
# read data frame from UCI machine learning database
... <- "..."
# use ';' delimiter, read_csv2 will not work as '.' is used as decimal points
... <- read_delim(..., ';')
```


#### Cleaning and Wrangling
After the data is read, the variable names are renamed to appropriate names.

Additionally, the quality variable is converted to a factor type, as it is a discrete variable.


```R
# rename column names for easier reference
colnames(...) <- c("...")

# convert quality to factor type
...<- mutate(...)

# preview ... data and see dimensions of df

```

'Table xx.xx: Preview of data set'

#### Splitting
Splitting the data involves some form of randomness. Thus, a seed is set for consistency.

The data is split with `SPLIT_PROPORTION` and strata `quality`.

#### Summary statistics of training data subset
Finding the number of `null` and `N/A` values, min, mean, max, and standard deviation.

#### Visualization of training data subset and determining appropriate predictors

The last part involves plots that are relevant to the objective.
The first plot is a distribution of the `quality` class variable.

### Data analysis
<a id='data_analysis'></a>
##### Data analysis will include:
- Initial visualization of the selected appropriate predictors with the class variable
- Training classification model using K-NN algorithm
- Training regression model using K-NN algorithm


#### Visualization of appropriate predictors and class variable


#### Training classification model with K-NN
We construct a training classification model with K-NN to determine the best value of k (code blocks are split so that individual code blocks can be run and skip run time).

##Expected outcomes and significance:

    What do you expect to find?
    What impact could such findings have?
    What future questions could this lead to?

## Discussion

[TEXT]

### References: 
1. <a id='ref_1'></a>
2. <a id='ref_1'></a>
