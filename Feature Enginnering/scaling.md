---
description: >-
  Feature scaling is used because we have different types or range of inputs so
  for getting result we have to scale them.
---

# Scaling

For example if we want to take 2 inputs of cgpa and IQ CGPA lies between 0 to 10 but IQ lies between 0 to 200 so we have to scale these in a fix order or in a fix range for getting efficient model&#x20;

There are two types of engineeriing scaling&#x20;

### <mark style="color:red;">1) Standardization scaling / Z-Score Normalization</mark>

_<mark style="color:orange;">**x' = x - mean(x) / SD**</mark>_&#x20;

<mark style="color:yellow;">x' refers the new col scaled data col and x refers originally value of that col and then we sub the mean of data and divide by SD means standard Deviation We find a new col data\_set in which we get all values are scaled and the mean of these values are 0 and standard deviation is 1</mark>

### <mark style="color:red;">2) Normalization scaling</mark>

Normalization is a techinque of data representation of data. Which converts the data of numeric columns to the scalable data set without changing the originally values of the data set&#x20;

### <mark style="color:red;">Types of Normalization scaling</mark>

#### <mark style="color:orange;">1)MinMax Scaling :- In this scaling we use different types of col\_data of numeric form and x = x(i) - x(min)//x(max) - x(min).This  range lie  in the range of  0 to 1. x(i) means originally value of the given data</mark>

<mark style="color:orange;">2)Mean Normalization :- Formula used in this is x = x(i) - x(mean)//x(max) - x (mean)  gives range of -1 to 1.</mark>

<mark style="color:orange;">3) MaxAbsolute Scaling :- x  = x(i)//x(max).</mark>

<mark style="color:orange;">It is used in sparse data (means a data in which no of zeros are more )</mark>

<mark style="color:orange;">4) Robust Scaling :- x = x(i) - x(median) // IQR</mark>&#x20;

<mark style="color:orange;">IQR means 75th percentile - 25th percentile</mark>

### <mark style="color:green;">Impact of outLier on our Scaling</mark>

### <mark style="color:blue;">When to use Standard Scaling</mark>

1\)K means =>Use the Euclidean distance measure&#x20;

2\)Nearest neighbour => Measure the distances between the pairs of samples and are influenced by the measurment units

3\)Principal components analysis =>Try to get feature with max variance

4\)Artifical Neural Network => Apply Gradient Descent

5\)Gradient Descent => Theta calcualtion becomes faster after scaling and learning rate in the update equation of the Stohastic Gradient Descent is the same for every parameter

### <mark style="color:red;">Normalization vs Standardization</mark>&#x20;

Is feature scalinngg require if you are  sured than Standardization is mostly used&#x20;

2\)&#x20;
