# Clustering Algorithm Assignment: DBSCAN, k-Means, and Hierarchical Clustering

## Coding Workflow

### Data Generation and Preparation

- Generated two synthetic datasets using scikit-learn:
  - `make_moons` (non-spherical clusters, demonstrates DBSCAN’s strengths)
  - `make_blobs` (spherical clusters with varying densities, highlights DBSCAN’s limitations)
  - Ensured datasets are suitable for direct input into clustering algorithms without additional preprocessing.

### Clustering Algorithms

- Implemented three clustering methods:
  - **DBSCAN:** Density-based clustering, excels at finding arbitrarily shaped clusters and handling noise.
  - **k-Means:** Partition-based clustering, effective for well-separated, spherical clusters.
  - **Hierarchical Clustering:** Agglomerative approach, flexible with cluster shapes but less scalable.

### Visualization

- Created clear scatter plots for each algorithm and dataset combination.
- Each plot includes:
  - Axis labels and descriptive titles
  - Color-coded clusters for interpretability
- Visualizations demonstrate where DBSCAN outperforms or underperforms compared to other methods.

### Comparative Analysis

- Evaluated and compared clustering results across all algorithms and datasets.
- Highlighted scenarios where DBSCAN is superior (e.g., non-spherical clusters, noise detection).
- Discussed DBSCAN’s failure cases (e.g., varying densities, parameter sensitivity).
- Summarized trade-offs influencing clustering method selection.

### Comparison Table

- Expanded the class comparison table to include DBSCAN.
- Provided concise, bullet-pointed strengths and weaknesses for each algorithm.
- Referenced visualizations as supporting evidence for key points.

### Code Organization

- All code is contained in `clustering_assignment.py` for ease of use and review.
- Functions are modular and well-documented with inline comments.
- The script is ready to run and will display all required visualizations.

## How to Run

1. **Install dependencies:**

2. **Run the script:**

3. **Output:**
    - Six labeled plots will be displayed:
    - DBSCAN, k-Means, and Hierarchical clustering  - results on both `make_moons` and `make_blobs`.
    - Use these plots in your report for analysis and comparison.

## Deliverables

- **main.ipynb:** Complete, well-documented code for all clustering analyses and visualizations.
- **Assignment3_Report.pdf:** 2–3 page report including:
  - DBSCAN algorithm overview
  - Comparative analysis with labeled visualizations
  - Expanded comparison table

## Objectives

- Understand and explain DBSCAN’s mechanics, parameters, strengths, and limitations.
- Compare DBSCAN with k-Means and Hierarchical Clustering using real visual evidence.
- Clearly communicate findings through both code and written analysis.