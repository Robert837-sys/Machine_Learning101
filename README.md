# Machine Learning 101

My personal learning log for machine learning, built up step by step with notes and runnable code. Each notebook pairs a short explanation of the concept with a working example, so the repo doubles as a study guide I can come back to.

> **Status:** 🚧 In progress. I'm updating this repo as I learn, so expect new notebooks and sections over time.

---

## Repository Structure

```
Machine_Learning101/
├── lesson1_ml.ipynb    # ML basics, statistics, data distributions, linear regression
├── SciPy.ipynb         # SciPy tutorial: optimization, sparse data, graphs, spatial data, stats tests
├── arr.mat             # MATLAB file generated in the SciPy notebook (scipy.io demo)
└── images/             # Diagrams used in the notebook notes
```

---

## What's Covered So Far

### 1. `lesson1_ml.ipynb`: ML Foundations

- **What ML is:** programs that learn from data to predict outcomes
- **Data types:** numerical, categorical, ordinal
- **Descriptive statistics:** mean, median, mode, standard deviation, variance
- **Percentiles:** using `np.percentile` to describe where values sit in a dataset
- **Data distributions:** uniform and normal distributions generated with NumPy, visualised with histograms
- **Scatter plots:** visualising relationships between two variables (including random data)
- **Linear regression:** fitting a line with `scipy.stats.linregress`, plus interpreting `r` (correlation), `p` (significance) and `std_err` (uncertainty of the slope)

### 2. `SciPy.ipynb`: Scientific Computing with SciPy

| Topic | What I practised |
|---|---|
| **Constants** | `scipy.constants` for units (metric/binary prefixes, mass, length, time, pressure, energy, etc.) |
| **Optimizers** | Finding roots of equations (`root`) and minimizing functions (`minimize` with BFGS); why ML is fundamentally about minimizing a function |
| **Sparse data** | `csr_matrix`, `.data`, `count_nonzero()`, `eliminate_zeros()`, `sum_duplicates()`, CSR to CSC conversion |
| **Graphs** | Adjacency matrices, connected components, Dijkstra, Floyd-Warshall, Bellman-Ford, depth-first and breadth-first traversal |
| **Spatial data** | Delaunay triangulation, convex hulls, KDTrees, distance metrics (Euclidean, cityblock/Manhattan, Hamming) |
| **MATLAB files** | Saving and loading data with `scipy.io.savemat` / `loadmat` |
| **Interpolation** | 1D, spline (`UnivariateSpline`) and radial basis function (`Rbf`, `RBFInterpolator`) interpolation, and how it relates to imputing missing data |
| **Statistical significance** | Hypothesis testing, t-test (`ttest_ind`), KS-test (`kstest`), `describe()`, skewness, kurtosis and `normaltest` |

---

## Tech Stack

- **Python 3**
- **NumPy**: numerical computing
- **SciPy**: optimization, statistics, sparse matrices, spatial algorithms
- **Matplotlib**: visualisation
- **pandas**: imported and ready for upcoming data work
- **Jupyter Notebook**: interactive notes and code

---

## Getting Started

```bash
# 1. Clone the repository
git clone https://github.com/Robert837-sys/Machine_Learning101.git
cd Machine_Learning101

# 2. (Optional) create a virtual environment
python -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate

# 3. Install dependencies
pip install numpy scipy matplotlib pandas jupyter

# 4. Launch Jupyter
jupyter notebook
```

Then open `lesson1_ml.ipynb` first and work through `SciPy.ipynb` after it.

---

## Roadmap

Things I plan to add as I keep learning:

- [ ] Multiple and polynomial regression
- [ ] Train / test split and model evaluation
- [ ] Scikit-learn fundamentals
- [ ] Classification (logistic regression, decision trees, k-nearest neighbours)
- [ ] Clustering (k-means, hierarchical)
- [ ] Feature scaling and encoding categorical data
- [ ] Working with real datasets end to end

---

## About

I'm Robert Owuor Agie (Roba), a Computer Science student specializing in Data Analytics at the University of Eldoret, Kenya.

- GitHub: [Robert837-sys](https://github.com/Robert837-sys)

---

## Notes

The learning material is based on tutorial-style lessons; all notebooks are my own working practice, with my own notes and edits added as I go.
