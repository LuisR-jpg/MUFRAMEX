# Pedestrian trajectory prediction

An application of deep generative modelling.

## Motivation

Infer future motions/intentions of human users in urban scenarios.

## Problem statement

### Conditions

Scenes populated with interacting agents.

Positions measured in a fixed frame.

### Problem

Given partial trajectories for agents and training examples, infer the trajectories in the near future. 

If possible: Include contextual data (maps, semantics...)

## Generative models and HTP

The predictive distributions should be multimodal. That means that it gives several paths that are potentially possible. 

## Solved with VAEs (Variational Auto Encoders)

Consists of using introducing a latent variable distribution that tries to match the real data.

Maximizing the likelihood of the data can be done by maximizing the ELBO term of VAE'S math representation.

## Challenges

Take into account the scene context

Generative models and uncertainty quantification

Scalable solutions

## Applications

Monitoring traffic intersections

Robot navigation

Safety around autonomous vehicles