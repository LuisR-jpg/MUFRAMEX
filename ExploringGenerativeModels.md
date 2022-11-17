# Exploring deep generative models

###### Lecture 4

## Generative adversarial networks

Two networks.

They're a case of sparse gradient.

### Generator

We have a neural network that takes noise and makes images.

### Discriminator

What this neural network does is telling whether a generated image belongs to our given dataset or not. 

Returns: $0 \leq p \leq 1$ where p is 1.0 if the network is sure that the image belongs to the dataset.

### How they work

These neural networks are adversaries, a generator tries to make similar images and the discriminator has to give feedback on whether they would belong to the dataset or not. 

Both keep training iteratively fighting against each other.

### How to layers

#### What size should I choose for my layer

Choose a power of two as a rule of thumb.

#### Is more layers better?

Nope, we're losing gradient on each layer, the more layers you have, the more you are worsening the values.

#### Should I choose a few layers then? 

Nope, we don't want a violent change of dimensions.

### Difficulties of GANs

They're super unstable, they can explode at any moment.

They're lazy. If it's not well set up, they will mode collapse. That is going for a single result without noise sensibility. It's harder to mess if you don't change the result.

### Hacks

LeakyReLU helps to keep information and not completely lose when we have something below zero.

If the learning rate is too big, GANs won't catch up. 