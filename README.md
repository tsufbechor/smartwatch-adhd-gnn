# Applying Graph Neural Networks on Smartwatch-Based Physiological Data for ADHD Medication Insights

This project leverages **Graph Neural Networks (GNNs)** to analyze physiological data collected from smartwatches to assess the effects of methylphenidate intake in children with ADHD. The study explores the application of GNNs to enhance the interpretation of time-series physiological data, aiming to improve predictions and insights into medication effectiveness.

## Overview

### Objective
The primary goal is to:
1. Assess the ability of GNNs to predict medication effects using trial data.
2. Examine if insights gained from trial data can be applied to observational datasets.

### Key Features
- **Physiological Monitoring:** Collects heart rate variability, motion levels, and autonomic nervous system metrics using advanced smartwatches.
- **Graph Neural Networks:** Structures time-series data into graph-based formats for enhanced analysis and predictions.
- **Predictive Modeling:** Utilizes Random Forest and Linear Discriminant Analysis (LDA) for evaluating GNN-augmented data.

## Methodology

1. **Data Collection:**
   - Participants: 15 children aged 6–16 with ADHD.
   - Devices: Smartwatches capturing physiological metrics such as heart rate, accelerometer, and gyroscope data.
   - Data Sources: 
     - Trial Data: Labeled data with medication intake records.
     - Observational Data: Unlabeled daily school observations.

2. **Graph Construction:**
   - Time-series data converted into graph structures with nodes representing data points and edges denoting sequential connections.
   - GNN layers: Graph Attention Convolution (GAT) layers with dropout and ReLU activation.

3. **Experiments:**
   - **Experiment 1:** Leave-one-out cross-validation within trial data to test GNN’s prediction performance.
   - **Experiment 2:** Generalize trial-derived insights to observational data.

## Results

- **Trial Data:** Significant improvement in prediction accuracy using GNN, with better separation of activity states in 4 out of 6 participants.
- **Observational Data:** Limited success in applying trial insights to observational datasets.

## Findings and Challenges

- **Key Insights:**
  - GNNs effectively enhance the interpretation of trial data.
  - Physiological changes during medication intake can be better captured using graph-based methods.
- **Challenges:**
  - Difficulty in generalizing insights from trial data to observational datasets.
  - Limited sample size affects model robustness.

## Future Directions

1. Expand dataset size for improved generalizability.
2. Explore advanced pre-processing techniques for better alignment of trial and observational data.
3. Incorporate additional contextual data, such as environmental or behavioral factors.
4. Evaluate alternative GNN architectures and machine learning models.

## Getting Started

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/roeiAv/Applying-Graph-Neural-Networks-on-Smart-watch-based-data-of-physiological-parameters.git
   cd Applying-Graph-Neural-Networks-on-Smart-watch-based-data-of-physiological-parameters
2. **Install Dependencies:**
  pip install -r requirements.txt

3. **Run the Analysis:** Use the provided scripts to preprocess data, construct graphs, train models, and evaluate results.

4. **Citation:** Bechor, T., Asulin, U., Kehat, Y., Avraham, R. (2024). Applying Graph Neural Networks on Smartwatch-Based Physiological Data for ADHD Medication Insights.

