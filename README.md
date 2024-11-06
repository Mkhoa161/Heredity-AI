# Heredity Probability Prediction

This project calculates the probabilities of gene inheritance and the presence of a genetic trait across multiple individuals based on family data. It uses a probabilistic model to predict gene inheritance patterns, taking into account both genetic probabilities and trait expressions. The model works with a CSV file containing individual genetic and trait information.

## Overview

This program calculates the joint probability of gene inheritance and the expression of a specific trait in a family tree. Given a dataset that contains information about individuals' parents, genes, and trait expressions, it applies the laws of probability to estimate the likelihood of each individual possessing certain genes and traits. The project involves:

- **Gene inheritance**: Probability of inheriting zero, one, or two copies of a gene.
- **Trait probability**: Probability of exhibiting a particular trait, given the number of inherited genes.
- **Family history**: Adjusting probabilities based on parent-child gene relationships.
- **Normalization**: Ensuring the final probabilities sum to 1 for each person’s gene and trait distributions.

The program is implemented in Python and can be run via the command line with a CSV file as input.

## Features

- **Gene Probability Calculation**: Estimates the likelihood of a person inheriting zero, one, or two copies of a gene.
- **Trait Probability Calculation**: Estimates the likelihood of a person exhibiting a trait, given the number of inherited genes.
- **Family History Integration**: Adjusts gene probabilities based on parental data (e.g., the mother and father’s genes).
- **Comprehensive Calculation**: Computes joint probabilities across multiple family members using a probabilistic model.

## Requirements

- Python 3.x
- `csv` and `itertools` modules (standard Python libraries)

## Installation

No installation is required. This project is a standalone Python script.

## Usage

Run the script via the command line, providing a CSV file that contains the data for your family. The CSV file should have the following columns:

- `name`: The name of the individual.
- `mother`: The name of the individual's mother (leave blank if unknown).
- `father`: The name of the individual's father (leave blank if unknown).
- `trait`: The trait value (either `0`, `1`, or blank for unknown).

Example:

```sh
python heredity.py family_data.csv
