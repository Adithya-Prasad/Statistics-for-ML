# What is Statistics?

_Statistics is the discipline that concerns the collection, organization, analysis, interpretation, and presentation of data. - Wiki_

It's the main ingredient of Data Analytics and Data Science. 

# Types of Statistics.
  
  ## 1. Descriptive Statistics
        _ It mainly summarizes(max, min, mean, median, range etc) the data from a population or sample. 

  ## 2. Inferential Statistics
        _ Used when we need to analyze the properties of the data and use a hypothesis or some statistical analysis to make predictions on a larger population of data or take decision/action on the data. 
        
        Examples: Hypothesis Testing, ANOVA, Chi-Square, Z Test, T-Test, F Test, Mann-Whitney Test, Regression Analysis, Time-Series Analysis, Etc.


# Population and Sample - Sampling Technique

  ## What is Population and Sample?
  ### Population:
         The entire dataset under investigation/analysis is the Population(N).
  ### Sample:
         A chunk of Population(n).
  
## Sampling:
  It is a statistical analysis of a fixed number of observations drawn from the whole population.

## Sampling Techniques

### 1. Simple Random Sampling:
Every data point/Individual has an equal chance of being selected

### 2. Systematic Sampling:
The first individual is randomly selected, and the others are selected using a fixed sampling interval(ith interval). There is no rule in choosing the interval.

Example: Let's say we have a dataset with 100 rows. We randomly select the first row (let's say 2nd row we selected). Then we will keep a fixed interval (say, every third row). My sample data will be taken from the following rows: 2, 5, 8, 11, 14...... 

### 3. Stratified Sampling:
Here the population is split into **non-overlapping groups**.

Example: If we are surveying the Job Satisfaction Index, Then if we consider Strata/layer/part of Engineers and Doctors there is a little chance that the Engineer's features/characteristics overlap with the Doctor's. There is no relationship between these two groups. So we will select some values from both the groups as samples from the population.

# Outliers

Outliers are the extreme values/numbers. 

- In statistics, an outlier is a data point that differs significantly from other observations. An outlier may be due to a variability in the measurement, an indication of novel data, or it may be the result of experimental error; the latter are sometimes excluded from the data set. (Wikipedia)

## Inter Quartile Range (IQR)

In descriptive statistics, the interquartile range is a measure of statistical dispersion, which is the spread of the data. The IQR may also be called the midspread, middle 50%, fourth spread, or H‑spread. It is defined as the difference between the 75th and 25th percentiles of the data. (Wikipedia)

IQR = Q3- Q2

Quartiles are defined as statistical measures that divide the given dataset into four equal parts: the first quartile (Q1), second quartile (Q2), and third quartile (Q3).

- Q1 is defined as the middle number between the smallest number and the median of the data set.
- Q2 is the median of the data.
- Q3 is the middle value between the median and the highest value of the data set.

Steps:
1. Sort the data
2. Find the median of total data/values/columns = Q2 = 50th Percentile
3. The Calculated Median divides given values into two equal parts as Lower Half and Upper half. these Lower Half and Upper half are determined as Q1 and Q3 parts.
4. Find Q1 (Median of the data before Q2) = 25th Percentile
5. Find Q3 (Median of the data after Q2) = 75th Percentile
6. Finally we subtract Q1 and Q3 to get IQR
   
![image](https://github.com/user-attachments/assets/9262980c-0aae-4981-be27-94fd88b778c5)

#### Upper and Lower Fence

The lower fence is the "lower limit" and the upper fence is the "upper limit" of data, and any data lying outside these defined bounds can be considered an outlier. The fences provide a guideline by which to define an outlier, which may be defined in other ways. The fences define a "range" outside which an outlier exists; a way to picture this is a boundary of a fence. It is common for the lower and upper fences along with the outliers to be represented by a boxplot

- Upper Fence = Q3 + 1.5* IQR
- Lower Fence = Q1 - 1.5* IQR

![image](https://github.com/user-attachments/assets/0fc85aed-e3df-4748-b8ed-85b62970ac26)


# Variables:

A variable can contain any value. 

There are two types of Variables.
1. Quantitative Variable (Measured numerically; Ex: Age, Marks)
2. Qualitative/Categorical Variables (Based on some characteristics we can categorize the variable; Ex: Gender, Blood Groups)

## Quantitative Variables:

Divided into:
1. Discrete variables: (Whole Number; These are fixed values; ex: Children in Family, Number of bank accounts, etc)
2. Continuous variables: (variable that can take on any value within a range. A continuous variable takes on an infinite number of possible values)

## Qualitative Variables: Also Called Variable Measurement Scales

4 types of Measured Variable:
1. Nominal(Named) Variable/data: (Gender, Boolean, Color, Types of Flower, etc)
2. Ordnial(ordered) variable/data: (Contains Hierarchy/Ranking; ex: Socio-Economic Status, Education Level, Satisfaction Index, etc.)
3. Interval : (range of values will be present and order also matters, Ex: Age brackets)
4. Ratio data: In a ratio scale, you can take a ratio of two values. For example, 40 kg is twice as heavy as 20 kg (taking ratios).
    Here are some examples of ratio variables:
   
        -  Temperature in Kelvin: The Kelvin scale has a true zero (0 K) where nothing can be colder. This allows you to calculate ratios of temperatures in the Kelvin scale.
    
        -  Age: Age has a true zero point, which means that a value of zero represents the absence of age.
   
        -  Number of children in a household: You can say that 4 children are twice as many as 2 children in a household.
   
        -  Years of work experience: You can say that 8 years is double 4 years of experience.

# Frequency Distribution:

A frequency distribution is a way to represent the number of observations within a given interval, either in a table or a graph. It shows how often a value occurs in an interval and the pattern of that frequency.

**Cumulative Frequency Distribution**

A cumulative frequency distribution is a way to represent the sum of a class and all the classes below it in a frequency distribution. It's a useful tool for determining how many observations are above or below a specific value in a data set.

## Usefull Graphs for Frequency:

We can use Bar Charts and **Histograms**

### What is a Histogram?

A histogram is an approximate representation of the distribution of numerical data.

Histogram is a display that indicates the frequency of specified ranges of continuous data values on a graph in the form of immediately adjacent bars.
*Interval* is a range of data in the dataset.

**Why Histogram?**: Used to summarize discrete or continuous data.
It provides a visual interpretation of numerical data by showing the number of data points that fall within a specified range of values (It is called **bins**)

## PDF (probability density function)

A probability density function (PDF) is the continuous version of a histogram, and it describes how probability density is distributed over a range of values.

**Definition**:
A PDF is a mathematical function that describes the likelihood of a random variable falling within a specific range.

**Visualization**:
A PDF is a smooth curve that shows the probabilities associated with different values of the random variable. 
Role
**PDFs are used to**: 
1. Estimate the probability of a variable falling within a specific interval 
2. Compare different distributions and understand their characteristics, such as variance and mean

### Kernel density estimation (KDE)

A non-parametric statistical technique that estimates the probability density function (PDF) of a continuous random variable.

**An idea of how KDE Works**: (Sourced from https://towardsdatascience.com/kernel-density-estimation-explained-step-by-step-7cc5b5bc4517 )

1. To get a sense of the data distribution, we draw probability density functions (PDF). We are pleased when data fit well to a common density function, such as normal, Poisson, geometrical, etc. Then, the maximum likelihood approach can be used to fit the density function to the data.
2. Unfortunately, the data distribution is sometimes too irregular and does not resemble any of the usual PDFs. In such cases, the Kernel Density Estimator (KDE) provides a rational and visually pleasant representation of the data distribution.
3. **The Kernel Function**: The key to understanding KDE is to think of it as a function made up of building blocks, similar to how different objects are made up of Lego bricks. The distinctive feature of KDE is that it employs only one type of brick, known as the kernel (‘one brick to rule them all’). The key property of this brick is the ability to shift and stretch/shrink. Each datapoint is given a brick, and KDE is the sum of all bricks.
4. KDE is a composite function made up of one kind of building block referred to as a *kernel function*.
5. The kernel function is evaluated for each datapoint separately, and these partial results are summed to form the KDE.
6. The first step toward KDE is to focus on just one data point. What would you do if asked to create a PDF for a single data point? To begin, take x = 0. The most logical approach is to use a PDF that is peaking precisely over that point and decaying with distance from it.
7. This Kernel is equivalent to a Gaussian distribution with zero mean and unit variance.


# Central Tendency

The measure used to define the center of the distribution.

1. Mean: Average of the data/values
2. Median: Useful when outliers are present. After **sorting** the numbers; For odd numbers, we need to consider the middle value and For even numbers, we need to take the average of the middle two values.
3. Mode: Most occurring data.

-> Notes: Median is calculated when there are some missing/undetermined/outliers values present in the data or the dataset is infinite.

# Measures of Dispersion

Dispersion = Spread

1. Variance:
  It is the measure of distance of each variable from the average value or mean value in its dataset.

   - Population variance:

![Population Variance Formula](https://github.com/user-attachments/assets/48b76782-6525-4fbb-b1c2-bbfa938eae3d)

   - Sample variance:

![Sample Variance Formula](https://github.com/user-attachments/assets/f7f4a3d3-9003-4949-9704-8618c01ce108)

2. Standard Deviation:

   Squareroot of Variance

   <img width="572" alt="image" src="https://github.com/user-attachments/assets/a0408490-d11b-4542-ac3b-28b4d217c2d6">

Variance and SD are all affected in the same way in the subject of the spread of the data. We use all these to present the data in a better manner.







# References:

Main Source: [Complete Statistics For Data Science In 6 hours By Krish Naik](https://www.youtube.com/watch?v=LZzq1zSL1bs)

[MathBitsNotebook](https://mathbitsnotebook.com/Algebra2/Statistics/STnormalDistribution.html)

[geeksforgeeks](https://www.geeksforgeeks.org)

(**Ongoing)



  
