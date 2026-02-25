# Unsupervised Machine Learning: K-Means Implementation

This project features a ground-up implementation of the **K-means Clustering Algorithm**. Unlike standard library implementations, this project focuses on the manual construction of the iterative clustering process to analyze the **Breast Cancer Wisconsin Dataset**.

## 🧠 Algorithm Mechanics
The implementation follows the iterative optimization strategy:
1. **Initialization:** Selecting initial centroids (handling the sensitivity of starting points).
2. **Assignment:** Using Euclidean distance to assign each data point to the nearest cluster.
$d(p, q) = \sqrt{\sum_{i=1}^{n} (q_i - p_i)^2}$
3. **Update:** Re-calculating centroids based on the mean of all points in the cluster.
4. **Convergence:** Repeating the process until cluster assignments stabilize.

## 📈 Project Goals
* **Data Processing:** Cleaning the Wisconsin Breast Cancer data (handling missing values and normalization).
* **Clustering Analysis:** Evaluating the effectiveness of $k=2$ (Benign vs. Malignant) through centroid movement.
* **Optimization:** Running multiple initializations to mitigate poor local minima results.

## 🛠️ Tech Stack
* **Python 3.x**
* **NumPy:** For vectorized distance calculations and centroid updates.
* **Matplotlib:** To visualize cluster distribution and final assignments.
