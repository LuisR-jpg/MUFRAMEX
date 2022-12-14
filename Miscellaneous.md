# Concepts and definitions

## Neural network

A neural network is a method in artificial intelligence that teaches computers to process data in a way that is inspired by the human brain. It is a type of machine learning process, called deep learning, that uses interconnected nodes or neurons in a layered structure that resembles the human brain.

## Recurrent neural network

A network with a loop, it processes information sequentially and the output from every time step is fed back to the network which acts as a sort of memory.

### Cons

This memory is limited, so information loss usually happens. This is called *gradient vanishing*.

## LSTM

Comes to solve the problem of RNNs. Using a *context vector* that is like a highway.

### Cons

- Take longer to train

- Require more memory

- Easy to overfit

- Dropout is much harder to implement

## GRU 

Similar to LSTM. GRU combines the forget and input gates into a single update gate.

It also combines the hidden state vector and the context vector into a single vector.

## Encoder Decoder architecture with Attention

Encoder is a series of LSTMS/GRUs to compress data, and uses a module attention before passing it to the decoder.

Attention multiplies the weights of the output of the decoder to focus on some specific features.

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

## Dropout 

Dropout is a technique where randomly selected neurons are ignored during training.

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

### [Super notes on learning](http://personal.cimat.mx:8181/~mrivera/cursos/temas_aprendizaje.html)

- [Seq2Seq](http://personal.cimat.mx:8181/~mrivera/cursos/aprendizaje_profundo/seq2seq/seq2seq.html)

- [VAE](http://personal.cimat.mx:8181/~mrivera/cursos/aprendizaje_profundo/vae/vae.html)

- [GAN](http://personal.cimat.mx:8181/~mrivera/cursos/aprendizaje_profundo/gan/gan.html)

### [Recurrent neural networks](https://www.youtube.com/watch?v=WEV61GmmPrk)

### [LSTM, GRU and Attention](https://medium.com/swlh/a-visual-and-intuitive-guide-to-lstm-gru-and-attention-8350518fa849)