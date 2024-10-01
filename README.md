# GenePhenMap: Gene and Phenotype Embedding Analysis

## Project Overview

**GenePhenMap** is a project focused on exploring relationships between genes and phenotypes using embedding techniques, PCA (Principal Component Analysis), K-Means clustering, and distance matrix calculations. The goal is to discover patterns and cluster gene-phenotype interactions to enhance our understanding of these biological connections.

## Features

- **Gene and Phenotype Embeddings**: Loaded from datasets containing high-dimensional vectors representing genes and phenotypes.
- **Principal Component Analysis (PCA)**: Dimensionality reduction applied to gene and phenotype embeddings for visualization.
- **K-Means Clustering**: Clustering of genes and phenotypes into groups based on their PCA-reduced features.
- **Distance Matrix Calculations**: Calculated distances between gene and phenotype embeddings to identify closest relationships.
- **Silhouette Analysis**: Evaluated the quality of clustering using silhouette scores.
- **Visualization**: Generated plots of gene and phenotype PCA projections, and connected closest pairs with lines to show their relationships.

## Project Structure

- `gene_embeddings.csv`: Contains embedding vectors for genes.
- `phenotype_embeddings.csv`: Contains embedding vectors for phenotypes.
- `opentargets_step2.for_llm.tsv`: Relationships between phenotypes and genes.
- `opentargets_step2.labels`: Ground truth labels for relationships.
- `gene_clustering_results.csv`: Output of gene clustering.
- `phenotype_clustering_results.csv`: Output of phenotype clustering.

## Key Scripts

1. **PCA Analysis**:
   - Performs dimensionality reduction on gene and phenotype embeddings using PCA.
   - Visualizes the PCA results with scatter plots.

2. **K-Means Clustering**:
   - Clusters the gene and phenotype embeddings into groups.
   - Visualizes the clusters and computes silhouette scores to evaluate clustering performance.

3. **Distance Matrix Calculations**:
   - Computes a distance matrix between the gene and phenotype PCA embeddings.
   - Identifies the closest phenotype for each gene and visualizes the connections.

4. **Elbow Method for Clustering**:
   - Generates elbow plots to determine the optimal number of clusters for both genes and phenotypes.

## Getting Started

### Prerequisites

- Python 3.x
- Required libraries:
  - `pandas`
  - `numpy`
  - `matplotlib`
  - `scikit-learn`
  - `scipy`
  - `hashlib`

### Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/GenePhenMap.git
   cd GenePhenMap
