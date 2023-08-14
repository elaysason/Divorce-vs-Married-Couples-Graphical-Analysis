# Divorce-vs-Married-Couples-Graphical-Analysis
Analyzing divorce and marriage dynamics using network analysis and graph theory.

## Overview
This project analyzes data related to divorce and marriage using network analysis techniques. The code is organized into several parts, including data preprocessing, graph creation, community detection, and statistical analysis. The main objectives of the project are to:

- Create networks based on couples' answers
- Detect communities within the networks using Louvain community detection
- Analyze and compare network properties between divorced and married couples
- Perform statistical tests to assess the separation between married and divorced couples

## Table of Contents
1. [Installation](#installation)
2. [Usage](#usage)
3. [Data](#data)
4. [Graph Creation and Analysis](#graph-creation-and-analysis)
5. [Community Detection](#community-detection)
6. [Statistical Analysis](#statistical-analysis)

## Installation
The project requires several Python libraries. To install the necessary packages, run the following command:


```
pip install pyspark python-louvain networkx pandas numpy matplotlib
```

## Usage
1. Run the provided code in a Python environment.
2. The code is structured into different sections:
   - Data loading and preprocessing
   - Network creation and visualization
   - Community detection using Louvain
   - Analysis of network properties
   - Statistical tests

## Data
The project uses a dataset named "divorce_data.csv." This dataset contains answers from couples, and the main task is to analyze divorce-related aspects. The dataset should have the following structure:

- Column: Divorce (0 for married, 1 for divorced)
- Columns: Q1, Q2, Q3, ... (Questions)

Note: The specific format and content of the dataset may vary based on the actual use case.

## Graph Creation and Analysis
The code includes functions for creating networks from couples' answers and visualizing the networks. It utilizes Pearson correlation, noise addition, and the Triangular Maximally Filtered Graph (TMFG) algorithm to create the network.

The network analysis includes the following steps:
- Creating networks for all couples, divorced couples, and married couples
- Analyzing network properties such as average clustering, modularity, shortest path length, centrality measures, and more

## Community Detection
The code employs the Louvain community detection algorithm to identify communities within the network. It calculates modularity to assess the quality of the detected communities.

Separate analyses for all couples, divorced couples, and married couples are provided.

## Statistical Analysis
The project performs statistical tests to assess the separation between married and divorced couples. It includes Kruskal-Wallis H tests for specific network properties and T-tests for modularity values.

## Results
The code generates various results and visualizations. These include:
- Visualization of the network of answers for all couples
- Visualization of the network with communities color-coded
- Analysis of global network properties (clustering, modularity, shortest path, etc.)
- Visualization of community graphs for individual communities
- Statistical test results for separation analysis


