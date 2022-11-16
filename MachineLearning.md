# Introduction to Machine Learning

###### Lecture 1.1

## 1. Introduction

### Machine learning

**Systems that learn to solve a problem from data and experience.**

The goal is to optimize a function that we don't know completely (because we usually have a sample only).

    If you're able to understand the difference between two or more things, you'll be able to predict an unknown one.


#### In ML we're interested in *optimality* and *quality*.

That is, we want the data to look like a normal distribution.

#### TODO: Insert here some notation and terminology

#### Errors and errors

When trying to get a curve that fits our point, we can face underfitting or overfitting, which is not good.

<div align = "center">
    <img align='center' src="https://github.com/LuisR-jpg/MUFRAMEX/blob/main/data/Fitting.png?raw=true"/>
    <br></br>
</div>

## 2. Examples of $\hat{Y}(x)$

i.e. Ways to achieve classification/regression.

### Nearest neighbor and KNN

Decide by voting (classification) or averaging (regression) what neighborhood a point in the space belongs to.

This is achieved by looking to the k closest neighbors.

### Regression model

For this model, we try to find a set of parameters $\vec{\beta}$ that maximizes the likelihood, that is, maximizing the probability to see what we just saw.

But finding a linear model is not always enough, because our data might not be a line. That is the starting point for neural networks.

### Neural network

#### Step 1. Define base functions.

We start composing functions by wrapping the notation we previously saw in the regression model ($x_i$ values multiplied by $\beta_i$).

The wrapper functions can be some basic operations. Like:

- Sign

- Identity

#### Step 2. Composition of base functions.

We start taking the output of base functions (neurons) as an input of others (neurons also).

And now we only have to $min_\beta\sum_i(y_i-f_\beta(x_i))^2$ by using $\triangledown f$ gradient descent with symbolic differentation and leads to applying a stochasting gradient method (gradient descent of subsamples).

## 3. Data and data

Data is super complex nowadays, we need numbers to optimize but our samples can be text or something else, so we have to find a way to transform it a vector.

Also, our data starts to become wider (more features) and shorter (not many samples).

## 4. Challenges

1. Uncertainty

2. Robustness and adversaries

    It's just matter of details to mess with our models. So we need a robust system.

3. Biases and fairness 

    If your dataset doesn't represent the population, wrong decisions can be made. 

4. Explainability and interpretability.

    Using perturbation methods can tell the importance or not importance of a method.

###### Lecture 1.2

## How to deal with graphs

- Galleries and cheatsheets are useful to see the tools you have at hand.

- It's important to know the differences.

    |Infographics               |Graphics                   |
    |---                        |---                        |
    |Self-contained             |Only gives support         |
    |Used once                  |As general as possible     |
    |Give a message/conclusion  |Are used for exploration   |

### Summaries

#### Scatter plot

You might not be seeing what you were thinking.

Our mind can lead to fast conclusions.

#### Mean, median, etc...

Pure numbers sometimes overlap when describing data.

<div align = "center">
    <img src="https://github.com/LuisR-jpg/MUFRAMEX/blob/main/data/EquivalentGraphics.jpeg?raw=true"/>
    <br>    
    All these graphs have the same mean
</div>
<br></br>

#### Boxplot and violinplot (seaborn)

Point out a glimpse of the shape of your data.

#### Pairplot (seaborn)

A matrix of graphs that helps to map each feature to see their relationships.

#### From two to higher dimensions

[Parallel coordinates](https://syntagmatic.github.io/parallel-coordinates/) (plotly)

Radarplot

#### Heatmap

It's a natural graph, easy to understand what it says.