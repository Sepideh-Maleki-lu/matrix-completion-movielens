# Matrix Completion for Movie Recommendation

This project was completed as part of the Numerical Linear Algebra course
in the Master in Financial Mathematics program at the University of Luxembourg.

The objective is to study matrix completion methods and apply them to
movie-rating prediction using the MovieLens dataset.

## Methods

Two main approaches are investigated:

- Nuclear norm minimization using FISTA and Singular Value Thresholding (SVT)
- Matrix factorization using a low-rank latent-factor model

## Dataset

The project uses the MovieLens dataset, containing user ratings for movies.
The observed ratings are divided into training and test sets to evaluate
how well the models predict missing ratings.

## Evaluation

The models are evaluated using relative recovery error on both training
and test data.

For nuclear norm minimization, different values of the regularization
parameter are tested.

For matrix factorization, different matrix ranks are compared.

## Main Findings

- Nuclear norm minimization provides good reconstruction performance but
  is computationally expensive because of repeated SVD computations.
- Matrix factorization is easier to implement and computationally lighter.
- The project also illustrates the importance of regularization,
  parameter selection, and avoiding overfitting.

## Files

- `Matrix_completion_project.ipynb` – Python implementation and experiments
- `matrix_completion_report.pdf` – Full project report

## Authors

- Sepideh Maleki-Roudposhti
- Cathérine Monoue Konga

University of Luxembourg  
Master in Financial Mathematics
