# 1. Measures of Central Tendency

**Measures of Central Tendency** are statistical metrics that describe the center or typical value of a dataset. They summarize data with a single value that represents the middle or center of its distribution.

## Types of Central Tendency

### 1. Mean
The arithmetic average of all data points.

**_Formula:_**
### $\frac{\sum{x_i}}{n}$
_where:_
- $x_i$ is ith observation, 1 ≤ i ≤ n
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
__________________________

# 2. Measures of Dispersion

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
#### $\sigma=\sqrt{\sigma^2}$

- **Sample Standard Deviation (s):**
#### $s=\sqrt{s^2}$
_________________________
# 3. Measures of Shape
## 1. Skewness 
Skewness can be defined as a statistical measure that
describes the lack of symmetry or asymmetry in the probability distribution
of a dataset. It quantifies the degree to which the data deviates from a
perfectly symmetrical distribution, such as a normal (bell-shaped)
distribution. Skewness is a valuable statistical term because it provides
insight into the shape and nature of a dataset’s distribution.

![](image/skewness.png)

## 2. Histograms 

A **histogram** is a graphical representation of the distribution of a dataset. It displays data using bars of different heights, where each bar groups numbers into ranges (bins).

### Key Features

- **Bins**: The intervals that represent the range of data values.
- **Height of Bars**: Indicates the frequency (count) of data points within each bin.
- **Continuous Data**: Histograms are used primarily for continuous data.

### Interpretation
- **Shape**: The overall shape (e.g., symmetrical, skewed) provides insight into the distribution.
- **Central Tendency**: The location of the peak(s) gives an idea of where most data points are concentrated.
- **Spread**: The width of the histogram shows the variability in the data.

![image](https://github.com/user-attachments/assets/433df3e1-32e5-4f69-adf1-3ba55e971f72)

## 3. Box plot
**Box plots** are used to show distributions of numeric data values, especially when you want to compare them between multiple groups. They are built to provide high-level information at a glance, offering general information about a group of data’s symmetry, skew, variance, and outliers.

![image](https://wac-cdn.atlassian.com/dam/jcr:3ecc2cdd-2878-4b9f-a853-f0d1782ad285/box-plot-construction.png?cdnVersion=2302)

### Quartiles
- **Quartiles** divide data into four equal parts:
  - **Q1 (1st Quartile)**: The 25th percentile.
  - **Q2 (2nd Quartile)**: The 50th percentile, also the median.
  - **Q3 (3rd Quartile)**: The 75th percentile.
- **Interquartile Range (IQR)**: The difference between Q3 and Q1, representing the middle 50% of the data.

## 4. Covariance and Correlation

**Covariance and correlation** are two statistical measures used to determine the relationship between two variables. Both are used to understand how changes in one variable are associated with changes in another variable.

#### Covariance
**Covariance** is a measure of how much two random variables change together. If the variables tend to increase and decrease together, the covariance is positive. If one tends to increase when the other decreases, the covariance is negative.

$$Cov(X,Y)=\frac{\sum(x_i-\bar{x})(y_i-\bar{y})}{N-1}$$

_where:_
- $x_i$ = Data value of x
- $y_i$ = Data value of y
- $\bar{x}$ = Mean of x
- $\bar{y}$ = Mean of y
- $N$ = Number of data value

#### Correlation
**Correlation** refers to the statistical relationship between the two entities. It measures the extent to which two variables are linearly related.



#### A. Pearson correlation coefficient
The **Pearson correlation coefficient** (r) is the most common way of measuring a linear correlation. It is a number between 
–1 and 1 that measures the strength and direction of the relationship between two variables.

$$Corr(X,Y)=\frac{Cov(X,Y)}{\sigma_x \sigma_y}$$

_where:_
- $\sigma_x$ = Standard deviation of X
- $\sigma_y$ = Standard deviation of Y

#### B. Spearman's rank correlation coefficient
**Spearman’s rank correlation** measures the strength and direction of association between two ranked variables. It basically gives the measure of monotonicity of the relation between two variables i.e. how well the relationship between two variables could be represented using a monotonic function.

$$\rho=1-\frac{6\sum d_i^2}{n(n^2-1)}$$

_where:_
- $d_i$ = Difference between the ranks of corresponding variables
- $n$ = Number of Observations
