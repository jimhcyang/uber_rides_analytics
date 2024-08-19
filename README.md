# Uber Rides Analytics

## Overview

This repository contains a collection of analyses and models for understanding Uber's pricing dynamics, customer behavior, and trip characteristics based on various datasets. The project involves analyzing Uber trip data, weather data, and exploring algorithms for predicting passenger flow and optimizing pricing strategies.

## Project Structure

- `best_models/`: Directory containing the best-performing models (daily_ride_prediction.ipynb).
- `data/`: Directory containing datasets used for analysis.
- `models/`: Directory for saved models and related files (daily_ride_prediction.ipynb).
- `output/`: Directory for generated output files and results (geodata_analysis.ipynb).
- `requirements.txt`: List of Python packages required for the project.
- `*.ipynb`: Jupyter notebooks with detailed analysis and results.
- `best_results.pkl`, `lstm_results.pkl`, `results.pkl`, `urgent_ride_classification_cluster.ipynb`, `urgent_ride_classification_pca.ipynb`, etc.: Various files and notebooks for analysis and results.

## Setup

### Create a Virtual Environment

```bash
python -m venv venv
source venv/bin/activate   # On Windows use `venv\Scripts\activate`
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

## Analysis and Tasks

### Analysis of Uber Platform and Competing Price Factors

1. **Data Analysis**: Analyzed a large dataset including Uber and Lyft trip data, weather data, and travel patterns.
2. **Key Investigations**:
   - Relationship between trip length and price.
   - Impact of weather on trip price.
   - Analysis of trip types and pricing.
   - Temporal and spatial characteristics of trip data, including migration patterns and weekday vs. weekend differences.

### Algorithm Executability Verification on Large Datasets

1. **Data Visualization**:
   - Used Folium to create heatmaps and visualizations for NYC trip data.
   - Generated heatmaps for starting and arrival points, and visualized travel trends.

2. **Machine Learning Models**:
   - Applied Lasso regression for feature selection.
   - Explored advanced algorithms like RNN, LSTM, and GRU for predicting passenger flow.
   - Analyzed model performance, feature importance, and prediction accuracy.

### Clustering and Classification

1. **Customer Segmentation**:
   - Used clustering algorithms to identify high-value and urgent Uber orders.
   - Evaluated different clustering methods, including K-means, DBSCAN, and hierarchical clustering.

2. **Model Evaluation**:
   - Integrated deep learning models to classify urgent orders based on profitability.
   - Employed PCA for dimensionality reduction and enhanced model performance.

## Notebooks

- `daily_ride_prediction.ipynb`: Analysis of daily ride patterns and predictions.
- `geodata_analysis.ipynb`: Exploration of geospatial data and mapping.
- `ride_price_analysis.ipynb`: Analysis of ride prices and their influencing factors.
- `urgent_ride_classification.ipynb`: Classification of urgent ride requests, best version.
- `urgent_ride_classification_cluster.ipynb`: Clustering analysis for urgent ride classification.
- `urgent_ride_classification_pca.ipynb`: PCA analysis for urgent ride classification.