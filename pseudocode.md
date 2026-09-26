---
title: "pseudocode"
author: "Lori Frager"
date: "2026-09-26"
output: html_document
---

## Pseudocode

### Step 1: Load the dataset

I need to read the data.  If it is a csv file, make sure you read it as csv.

Data = read.csv("dataset.csv")


### Clean the data

First make sure each column is in the right kind of data. Factor, decmeil number, etc. 
Second, decide how you will handle missing values?  Should the be skipped or put in an average number.
How the null values will be handled.  Should they be included in the data or those lines of code removed.
Do we have duplicates? Are they supposed to be included?
Will the data need to be normalized for a cleaner representation of the data?


### Caclulate summary statistics

Summary and sd.  I'm going to use the Iris data.

summary(iris)
sd(iris)

The summary will give me the mean, median, the min and max, and the 1st and 3rd quartile.  The sd gives me the standard deviation.

### Create a visualization

Here is a boxplot on the Iris data set comparing the sepal length to the class. (species)

plot(iris$sepal_length ~ class)

I am comparing the sepal length in all the classes (species).  Each class will have it's own plot showing
the median, the first and third quartile, any outliers and the max and min range of the data. 

### Interpret results

Looking at the box plots.  Is one variety higher than the other? Do they have outliers?  
Are the simular in their ranges? Is the medean in the middle of the box or closer to one end?  Are their medians close to the same? The answer to these questions, will tell us how simular/different the different varieties of the flowers are. 
