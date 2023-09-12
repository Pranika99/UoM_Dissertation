# University of Manchester Dissertation Project
# Title- Graph Based Semi-Supervised Learning

Welcome to the project repository that investigates the field of Graph-based Semi-Supervised Learning (GSSL), a discipline of Machine Learning that utilises both labelled and unlabelled data to predict missing labels. It is used in scenarios where labelling is resource-intensive and time-consuming.

# Objective
The aim is to understand important role of regularity of solutions in Graph Laplacian learning and how p-Laplace learning can help to improve the smoothness of Laplacian learning solutions, especially when only a few labelled data points are available. It closely examines the Laplace learning approach which spreads labels across the graph using a harmonic extension mechanism. However, in case of a very low label rate, the method leads to the formation of “spikes” exhibiting irregularity of solutions.

# Dataset
The experimentation uses the FashionMNIST dataset for the analysis. Link to dataset- https://github.com/zalandoresearch/fashion-mnist

# Package and Version
GraphLearning package- 1.2.7
Link to the GraphLearning package- https://github.com/jwcalder/GraphLearning

# Methodology
The work employs four different Graph based Semi-supervised learning models to examine the regularity of Laplacian solutions. The models are as following:
1. Model 1 studies the graph Laplacian for 2-Dirichlet energy using raw dataset. Combinatorial Laplacian (L=D-W) has been used here.
2. Model 2.1 explores the graph Laplacian for 2-Dirichlet energy using Combinatorial Laplacian. The dataset is pre-processed using Variational Autoencoders.
3. Model 2.2, similar to Model 2.1 utilises Random Walk Laplacian to explore solutions of Graph Laplacian.
4. Model 3 (p-Laplacian model with p=10) acts as an optimisation model for the Laplacian learning.

# Key Findings
For Laplacian learning, the formulation of mathematical relationships based on the random walk approach promotes a smooth solution by suggesting an inverse relationship between the error and the product of the probability of hitting a labelled node and the transition probability between a labelled and unlabelled node. Moreover, the regularity of Laplacian learning successfully improves with the use of p-Dirichlet energy.
