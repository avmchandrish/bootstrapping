# Bootstrapping
As data scientists and, by extension, statisticians, our job is to perform tests and create models about a *target population* from data collected on a *sample* of that population. 

Let's say we want to find out the percentage of people in the world who like mint ice cream. We can survey a group of people of maybe 100 people to find out that 89% are mint ice cream enjoyers. Concluding that 89% of all 7 billion people on Earth enjoy mint ice cream is not good practice. However, continuing to survey people until all 7 billion opinions have been recorded is close to impossible, incredibly time-consuming, and expensive. This is where **bootstrapping**  comes in as a solution to our problem. 

## A quick introduction

**Bootstrapping** is a traditional statistics technique used to solve the problem of inadequate data. The idea is to generate a bootstrapped sample of the original data many, many times to imitate the generation of new data. 

> The term **bootstrapping** comes from the American idiom *"to pull oneself up by the bootstraps"*, which means to do something by your own efforts and resources, without outside help. 

In the same way, bootstrapping is a useful technique in statistics and data science, because it does not require time-consuming (and often, expensive) recollection of data, or repeated surveys. 

## Methodology
To bootstrap, we perform the following steps: 

1. Resample the existing data uniformly, and with replacement, for the total number of observations in the dataset.
2. Calculate a statistic (e.g. mean, median) for that bootstrapped sample. 
3. Record the result.
4. Repeat steps 1-3 many times. Often, bootstrapping can occur 1,000 - 100,000 times.

*([this StatQuest video](https://www.youtube.com/watch?v=Xz0x-8-cgaQ&ab_channel=StatQuestwithJoshStarmer) is helpful for both its visualizations and explanations)*

**Note:** Each bootstrapped dataset preserves the distribution of the original dataset. This follows from sampling uniformly and with replacement.

After performing the above steps to our satisfaction, we can reexamine the aggregate of our recorded statistics. The amount of data gathered should be adequate for us to understand the true population statistic. That is, if our initial sample set of data is an accurate reflection of the population, our result should return a true population mean, median, etc.

## Applications

Bootstrapping is an incredibly versatile tool for improving statistical inference. Next, we discuss three example applications.

### 1. Means



### 2. Medians

### 3. Decision Trees and Random Forests

*(to read more about applications of bootstrapping, as well as different types, such as non-parametric, Bayesian, etc. bootstrapping, check out [Jillian Green's Medium article](https://jillian-green.medium.com/applications-of-bootstrapping-8240da9df6d7))*
