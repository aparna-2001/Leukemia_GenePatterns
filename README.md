# Leukemia_GenePatterns

A comprehensive analysis of the Golub leukemia gene expression dataset using Python, demonstrating a complete data analysis pipeline from preprocessing to dimensionality reduction.

## Overview

This project analyzes high-dimensional gene expression data from leukemia patients to identify patterns and relationships between different cancer types. Using Principal Component Analysis (PCA) with Singular Value Decomposition (SVD), the analysis reduces the complexity of thousands of gene expressions into a small number of interpretable components that capture the major sources of variation.

The reduced-dimensional representation is then used for unsupervised clustering, including K-Means clustering to group samples based on global expression similarity and hierarchical clustering to visualize relationships among samples through dendrograms. These clustering approaches help reveal natural groupings of cancer samples and highlight similarities and differences in their underlying gene expression profiles.

## Dataset

The Golub leukemia dataset is a classic benchmark in bioinformatics, containing gene expression measurements from patients with acute lymphoblastic leukemia (ALL) and acute myeloid leukemia (AML). This high-dimensional dataset provides an excellent case study for dimensionality reduction techniques.

## Features

- **Data Preprocessing**: Cleaning and preparing gene expression data for analysis
- **Exploratory Data Analysis**: 
  - Mean expression analysis across genes
  - Variance exploration to identify highly variable genes
  - Statistical summaries and visualizations
- **Dimensionality Reduction**: 
  - PCA implementation using Singular Value Decomposition (SVD)
  - Visualization of principal components
  - Pattern identification in gene expression space
- **Visualization**: Clear, publication-quality plots using matplotlib and seaborn
- **Clustering** : Kmeans clustering and Hierarchical clustering(dendrogram) using scikit-learn

## Technologies Used

- **Python 3.x**
- **NumPy**: Numerical computations and array operations
- **Pandas**: Data manipulation and analysis
- **Matplotlib**: Data visualization and plotting
- **Seaborn**: Statistical data visualization (heatmap)
- **Scipy** : scientific computing (hierarchical clustering)
- **scikit-learn** : clustering 

## Installation

1. Clone the repository:
```bash
git clone https://github.com/aparna-2001/Leukemia_GenePatterns.git
cd Leukemia_GenePatterns
```

2. Install required packages:
```bash
pip install numpy pandas matplotlib seaborn
```

Or using a requirements.txt file:
```bash
pip install -r requirements.txt
```

## Usage

```python
# Run the main analysis script
python leukemia_analysis.py
```

The analysis pipeline will:
1. Load and preprocess the gene expression data
2. Compute mean and variance statistics
3. Perform PCA using SVD
4. Generate visualizations of the results


```

## Key Analysis Steps

### 1. Data Preprocessing
- Handling missing values
- Normalization/standardization
- Data quality checks

### 2. Exploratory Analysis
- Computing gene-wise mean expressions
- Identifying highly variable genes
- Statistical distribution analysis

### 3. PCA via SVD
- Decomposing the gene expression matrix
- Identifying principal components
- Variance explained analysis
- Sample projection onto PC space

## Results

The analysis reveals:
- Distinct clustering patterns between ALL and AML samples
- Key genes contributing to cancer type differentiation
- Reduced-dimension representation preserving biological variability

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Golub et al. for the original leukemia dataset
- The bioinformatics community for open-source tools and methods

## References

Golub, T. R., et al. (1999). "Molecular classification of cancer: class discovery and class prediction by gene expression monitoring." *Science*, 286(5439), 531-537.

## Contact

For questions or feedback, please open an issue on GitHub or contact [your email].

---

**Note**: This project is for educational and research purposes only.
