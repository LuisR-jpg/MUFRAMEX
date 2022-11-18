# Concepts and definitions

## Neural network

A neural network is a method in artificial intelligence that teaches computers to process data in a way that is inspired by the human brain. It is a type of machine learning process, called deep learning, that uses interconnected nodes or neurons in a layered structure that resembles the human brain.

## Adam algorithm

Adam is a replacement optimization algorithm for stochastic gradient descent for training deep learning models.

## Latent space

The latent space is simply a representation of compressed data in which similar data points are closer together in space. Latent space is useful for learning data features and for finding simpler representations of data for analysis.

## LR/Step

Both stand for the size of steps or the speed of movement when optimizing a function.

It's *step* in machine learning.

It's *learning rate* in deep learning.

## Generative model 

En probabilidades y estadística, un modelo generador es un modelo para generar valores aleatorios de un dato observable, típicamente dados algunos parámetros ocultos. Este especifica una distribución conjunta sobre una secuencias de etiqueta. 

# Coding challenge

We're given sequences of actions, poses.

It was created by 11 professional actor subjects. Doing 15 scenarios.

## Objectives

Predict human motion. $\hat{Y}$ returns the final sequence.

## Dataset

[Dataset](http://vision.imar.ro/human3.6m/description.php)

Raw data has 99 values per frame.

First three are global translation. The rest are joint angles.

Selection process (see function normalization_stats()) that selects 54 of these variables. (It removes the ones that don't vary)

Normalization process (see function normalize_data()) to center the data and set them to unitary variance.

The steps are done in read_all_data()

## Base model

This can be cast as a regression problem.

[Model](https://github.com/cimat-ris/human-motion-prediction-pytorch)

## Presentations

- 8 minutes presentation + 2 minutes question on Saturday.

- Should sum up your strategy + your results.

- At least 3 different presenters.

# Resources 

Cool ideas, knowledge, sources found during the school.

## PhDs areas

- PhD of Mathematics of computational models and applied physics

- PhD on knowledge graphs 

## People

Ulises Moya Sanchez (eduardo.moya@jalisco.gob.mx)

## Notes 

[Super notes on learning](http://personal.cimat.mx:8181/~mrivera/cursos/temas_aprendizaje.html)