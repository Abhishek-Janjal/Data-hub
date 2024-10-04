# Statistics

**Statistics** is a branch of mathematics that deals with the collection, analysis, interpretation, presentation, and organization of data. It provides tools for making informed decisions based on data by identifying patterns, relationships, and trends.
## Significance of Statistics in Data Science/Machine Learning

In Data Science and Machine Learning, statistics play a crucial role in:

- **Data Analysis:** Helps in understanding and interpreting the underlying patterns in data.
- **Model Development:** Provides methods to make inferences about data and helps in building predictive models.
- **Hypothesis Testing:** Facilitates the testing of assumptions and validating models.
- **Decision Making:** Assists in making data-driven decisions by quantifying uncertainty and risk.
___________________________________
# Types of Statistics

<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRypl66gx5dsYqvj15qKq1Do5iQMbVWp3Ml3g&s" alt="Statistics vs Machine Learning" height="300px" width="500px">

Statistics can be broadly classified into two types:

### 1. [Descriptive Statistics](content/descriptive.md)

Descriptive statistics summarizes and describes the features of a dataset. It helps in understanding the basic characteristics of the data through numerical summaries, graphs, and charts.

**Key Components of Descriptive Statistics:**
- **Measures of Central Tendency:** Mean, Median, Mode
- **Measures of Dispersion:** Range, Variance, Standard Deviation
- **Measures of Shape:** Skewness, Kurtosis
- **Data Visualization:** Histograms, Box plots, Bar charts

**Examples of Descriptive Statistics:**
- **Mean:** The average of a set of numbers.
- **Median:** The middle value when the numbers are arranged in order.
- **Standard Deviation:** A measure of the amount of variation or dispersion in a set of values.
- **Histogram:** A graphical representation of the distribution of data.

### 2. Inferential Statistics

Inferential statistics uses a random sample of data taken from a population to describe and make inferences about the population. It allows us to make predictions or generalizations about a population based on a sample.

**Key Components of Inferential Statistics:**
- **Estimation:** Point Estimation, Confidence Intervals
- **Hypothesis Testing:** Null and Alternative Hypotheses, p-value, t-tests, chi-square tests
- **Regression Analysis:** Linear Regression, Logistic Regression
- **Correlation:** Pearson correlation, Spearman rank correlation

**Examples of Inferential Statistics:**
- **Confidence Interval:** An estimated range of values which is likely to include an unknown population parameter.
- **t-test:** A statistical test used to compare the means of two groups.
- **ANOVA (Analysis of Variance):** A method for comparing multiple group means to see if at least one is different.
- **Regression Analysis:** Used to predict the value of a dependent variable based on the value of one or more independent variables.
___________________________________
# Population vs Sample Data in Statistics


| Feature                | Population                              | Sample                                  |
|------------------------|-----------------------------------------|-----------------------------------------|
| **Definition**         | Entire group of interest                | Subset of the population                |
| **Size**               | Larger (often denoted by N)             | Smaller (denoted by n)                  |
| **Parameters**         | Population parameters (e.g., μ, σ²)     | Sample statistics (e.g., x̄, s²)        |
| **Data Collection**    | More complex, costly, and time-consuming| Easier, less expensive, and faster      |
| **Comprehensiveness**  | Includes all members                    | Includes only selected members          |
| **Example**            | All employees in a company              | 100 employees selected for a survey     |
_______________________________________
# Measures of Central Tendency

**Measures of Central Tendency** are statistical metrics that describe the center or typical value of a dataset. They summarize data with a single value that represents the middle or center of its distribution.

## Types of Central Tendency

### 1. Mean
The arithmetic average of all data points.

**_Formula:_**
### $\frac{\sum{X_i}}{n}$
_where:_
- $X_i$ is ith observation, 1 ≤ i ≤ n
- _n_ is Number of observations

### 2. Median
The middle value in a sorted dataset. If the number of observations is even, the median is the average of the two middle numbers.

**_Formula:_**

_For Even_
$M=(\frac{n+1}{2})^{th}$

_For Odd_
$M=\frac{(\frac{n}{2})^{th}+(\frac{n}{2}+1)^{th}}{2}$

_where:_
- _n_ is Number of observations

### 3. Mode
The value that appears most frequently in the dataset.


## Summary

- **Mean:** Best for data without extreme outliers, sensitive to outliers.
- **Median:** Best for skewed data or data with outliers.
- **Mode:** Best for categorical data or identifying the most frequent value.

_________________________________________________
# Measures of Dispersion

<p align="center">
  <img src="https://media.geeksforgeeks.org/wp-content/uploads/20230810105933/measure-of-depression.png" alt="Measures of Dispersion"/>
</p>


**Measures of Dispersion** quantify the spread or variability within a dataset. They provide insights into how much the data points differ from the central tendency measures (like the mean or median).

## 1. Variance

The average of the squared differences between each data point and the mean.
**Formulas:**
- **Population Variance (σ²):**
$$\sigma^2=\frac{\sum(X_i - \mu)^2}{N}$$

- **Sample Variance (s²):**
$$s^2=\frac{\sum(X_i - \bar{X})^2}{n-1}$$ 

_where:_
- $X_i$ = each data point
- $\mu$ = population mean
- $\bar{X}$ = sample mean
- $N$ = size of the population
- $n$ = size of the sample

## 2. Standard Deviation

The square root of the variance, representing the average distance of each data point from the mean.
**Formulas:**
- **Population Standard Deviation (σ):**
##### $\sigma=\sqrt{\sigma^2}$

- **Sample Standard Deviation (s):**
##### $s=\sqrt{s^2}$

____________________________________________

# Variable in Statistics

A **variable** is a characteristic or attribute that can take on different values or categories. Variables are fundamental in statistics as they represent the data that is analyzed.

## Types of Variables

1. **Quantitative Variables**: 
   - **Continuous**: Can take on any value within a range (e.g., height, weight).
   - **Discrete**: Can only take on specific values, usually counts (e.g., number of children).

2. **Qualitative Variables**: 
   - **Nominal**: Categories without a natural order (e.g., gender, eye color).
   - **Ordinal**: Categories with a natural order (e.g., ranking, education level).
