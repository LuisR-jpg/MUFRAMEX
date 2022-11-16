# Coding challenge

We're give sequences of actions, poses.

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