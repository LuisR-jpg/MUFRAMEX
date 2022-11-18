# How to take portraits of people who do not exist

## Steps for data generation

We need to estimate the data distribution $P(x)$ and to generate samples $x ~ P(x)$ such that:

1. The generated images are similar to those of the training database.

2. The generator is parameterized by a vector of latent variables with a known distribution and simple to sample.

3. The generated images are not present in the training database.

## Ways to achieve it 

### Autoencoder

It's an architecture that compresses the data and it tries to decompress it back to the original; we should expect a pretty similar result.

The problem with it is that at the very center, the values are unbounded, so the data is a cloud of points with empty spaces.

### Variational autoencoder

This is the result of normalizing the encoded data into a Gaussian Function and that generates a smooth, filled cloud of data.

Having this property allows us to take samples out of that distribution.

Taking samples allows us to parameterize, and getting to know what exact variables change what in a face or the output.

They achieve the results but with a huge lost of details, so:

#### Pix2Pix

This approach is a GAN proposed to give details to an image.

This gives details but the result is horrible, creepy.

#### Transformers

They're used to borrow information from other examples to work out the previous results

## Resources

[Super notes on learning](http://personal.cimat.mx:8181/~mrivera/cursos/temas_aprendizaje.html)