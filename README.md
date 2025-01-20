# smartwatch-adhd-gnn
A Graph Neural Network approach for analyzing smartwatch-based physiological data to predict methylphenidate intake effects in children with ADHD. This research combines wearable technology data with advanced deep learning techniques to understand medication responses through physiological biomarkers
# Overview
This project applies Graph Neural Networks (GNNs) to analyze physiological data collected from smartwatches worn by children with ADHD. The goal is to predict and understand methylphenidate intake effects using various physiological parameters including heart rate variability, movement levels, and sympathetic nervous system arousal.
# Research Context

Study focused on 15 children with ADHD (ages 6-16, mean age 11.10 ± 2.69)
Data collected through smartwatch sensors during medication administration
Collaboration with Iluria Ltd., a digital health software startup

# Key Features

Processing of multimodal smartwatch sensor data (accelerometer, heart rate, gyroscope)
Graph Neural Network implementation for time-series physiological data
Two experimental approaches:

Leave-one-out cross-validation on trial data
Transfer learning from trial data to observational data



# Data Collection
Sensor Data

Accelerometer (x, y, z)
Heart rate monitoring
Gyroscope (x, y, z)
Continuous physiological measurements

# Data Types

Trial data (6 participants) with labeled medication states
Observational data (9 participants) from regular school days

# Data Processing

Time-series to graph conversion
Feature extraction for GNN nodes
Temporal edge creation

# Model Architecture

Three-layer GNN with Graph Attention Convolution (GAT)
Dropout regularization
RELU activation functions

# Evaluation Methods

Random Forest prediction with AUC curve analysis
Linear Discriminant Analysis (LDA) for activity state separation
Weekly consolidated confidence graphs

# Results

Improved prediction performance in trial data analysis
Enhanced separation of activity states in 4/6 participants
Limited success in generalizing to observational data
