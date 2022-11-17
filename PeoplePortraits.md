# How to take portraits of people who do not exist

## Steps for data generation

We need to estimate the data distribution $P(x)$ and to generate samples $x ~ P(x)$ such that:

1. The generated images are similar to those of the training database.

2. The generator is parameterized by a vector of latent variables with a known distribution and simple to sample.

3. The generated images are not present in the training database.

## Ways to achieve it 

### Autoencoder

It's an architecture that compresses the data and it tries to decompress it back to the original. We should expect a pretty similar result.

It needs an extra piece that is called sampler and it's at the center.

    Trick
    By modifying the values given to the sampler, we can achieve smooth transitions from faces to faces.

### VAE

They achieve the results but with a huge lost of details, so:

#### Pix2Pix

This approach is a GAN proposed to give details to an image.

This gives details but the result is horrible, creepy af.

#### Transformers

They're used to borrow information from other examples to work out the previous results

## Resources

[Super notes on learning](http://personal.cimat.mx:8181/~mrivera/cursos/temas_aprendizaje.html)