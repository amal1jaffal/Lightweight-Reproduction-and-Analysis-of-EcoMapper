# Lightweight Reproduction and Analysis of EcoMapper
A lightweight reproduction and experimental analysis inspired by EcoMapper, investigating how satellite imagery and environmental variables contribute to land-cover classification using a multimodal diffusion-based approach.

The project focuses on understanding the relative contribution of Sentinel-2 satellite imagery and climate/environmental variables, while analyzing model performance and overfitting in a lightweight experimental setting.

# Key Finding

In my reproduction experiments, satellite imagery provided stronger land-cover information than climate variables alone. The initial multimodal model also showed substantial overfitting, highlighting the challenges of combining heterogeneous environmental data in a relatively small experimental setup.

# Project Overview

This project reproduces a lightweight version of the core idea behind EcoMapper rather than attempting to reproduce the complete original system.

The main objectives were to:

Explore the use of Sentinel-2 satellite imagery for land-cover classification.
Investigate whether climate and environmental variables provide complementary information.
Experiment with a lightweight diffusion-based model.
Compare the information provided by different input modalities.
Analyze model behavior, generalization, and overfitting.
Build a reproducible dataset and metadata pipeline for environmental machine learning.

The project sits at the intersection of:

Remote Sensing · Environmental Geoscience · Machine Learning · Computer Vision · Geospatial Data Science
# Research Questions

The experiments were designed around three main questions:

How informative is satellite imagery for land-cover classification?
Can climate/environmental variables provide useful complementary information?
Does combining both modalities improve generalization, or does the additional complexity introduce overfitting?

# Methodology

The dataset combines satellite imagery with environmental and land-cover information.

Input Data
Sentinel-2 satellite imagery
Climate/environmental variables
Geographic metadata
Temporal information
Land-cover labels

Each satellite image is paired with a corresponding metadata record containing temporal, geographic, environmental, and land-cover information.

Model

A lightweight diffusion-based architecture was used to investigate multimodal conditioning.

# Dataset Download: https://mediatum.ub.tum.de/node?id=1767651

The dataset contains:

2.9 million Sentinel-2 images
15 land cover classes
6 years of monthly observations
Global geographic coverage
Associated climate metadata for each image
Each satellite image is paired with a metadata .csv file that stores temporal, geographic, environmental, and land-cover information used for training and conditioning.

# Results

The experiments indicate that satellite imagery contained stronger land-cover information than climate variables alone.

The initial multimodal experiments also revealed substantial overfitting, suggesting that simply adding environmental variables does not necessarily lead to better generalization.

# Limitations

This project is intentionally a lightweight reproduction and should not be considered a full reproduction of the original EcoMapper system.

Important limitations include:

Reduced model size
Limited computational resources
Simplified training setup
Potential class imbalance
Limited hyperparameter optimization
Risk of geographic and temporal distribution shift
Significant overfitting in the initial multimodal experiments

These limitations are important when interpreting the reported results.
