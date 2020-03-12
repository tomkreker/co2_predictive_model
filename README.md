# Predicting CO<sub>2</sub> Emissions

## Overview
The aim of this project was to create a predictive model using a Bayesian approach to predict CO<sub>2</sub> emissions until 2058 based on measurements taken at the Mauna Loa Observatory between 1958 and 2019. The model was only refined to a fairly satisfactory level and the report specifies several areas through which it could have been further improved. The project was a part of a course titled *Modern Computational Statistics*, taken during Fall semester of 2019.

## Contents
1. A PDF report that summarizes the approach, implementation, and results.
2. A Jupyter Notebook with the code.
3. A CSV file with the data.

The code and analysis cover the following topics:
1. Introducing a first 'example' model
2. Adding a quadradic term
3. Adding an inner-cosine term
4. Discussing possible extensions
5. Producing predictions

## Model
The final likelihood function is made of four components:
1. A quadradic long-term trend.
2. A cosine-based seasonal variation component.
3. An inner cosine function to account for the assymtery of the cycles.
4. Random noise.

Full specification of the priors, likelihood, and the full joint probability over all parameters can be found in the report.

## Code Structure
The code is divided to several sections: 
1. Loading the data.
2. Building a first model and obtaining results via Stan.
3. Refining the first model with an inner-cosine function via Stan.
4. Obtaining predictions for the next 40 years. 
