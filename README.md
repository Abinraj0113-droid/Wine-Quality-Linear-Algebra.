# Wine Quality Analysis using Linear Algebra & Probability

## Project Overview
This project applies fundamental techniques from Linear Algebra and Probability to analyze the structural chemical properties of red wine and evaluate how these features relate to overall wine quality scores.

## 1. Data Preprocessing Steps
* **Dataset Used:** Red wine quality dataset containing 1,599 rows and 12 columns.
* **Data Cleaning:** Handled missing/null entries dynamically by replacing them with the calculated mean value of their respective columns to maintain statistical consistency.

## 2. Core Analysis Tasks
* **Vector Extraction:** Extracted the `alcohol` and `citric acid` properties into separate 1D NumPy arrays/vectors for linear algebraic evaluation.
* **Covariance Matrix:** Built a feature matrix space using `alcohol` and `density`. The covariance matrix was calculated using Python's `np.cov(X.T)` to understand how these features vary together.
* **Eigen Decomposition:** Performed eigen decomposition on the covariance matrix using `np.linalg.eig` to calculate the top 2 eigenvalues and their corresponding eigenvectors, identifying the principal components of variance.

## 3. Graphical Representations & Insights
* **Most Common Quality:** The most common wine quality score in the dataset is **5**.
* **Probability Distribution:** The quality scores follow a discrete, bell-shaped distribution centered tightly around average scores (5 and 6). High-quality (7 or 8) or low-quality (3 or 4) wines occur with significantly lower statistical probability, highlighting that exceptional profiles are rare events on the tails of the distribution.
* **Visualizations:** The Jupyter Notebook includes a generated countplot visualization displaying the distribution frequency of these wine quality categories.

## How to Run the Workspace Locally
1. Clone this repository.
2. Install dependencies: `pip install pandas numpy matplotlib seaborn`
3. Launch Jupyter Notebook and run all cells in your notebook file.
