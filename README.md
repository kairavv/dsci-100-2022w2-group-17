# [Project Question]
## Introduction
[Text]
## Methods
[Text]
### Preliminary exploratory data analysis
<a id='pre_data_analysis'></a>
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

## Discussion

[TEXT]

### References: 
1. <a id='ref_1'></a>
2. <a id='ref_1'></a>
