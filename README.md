# Affinity Propagation Clustering from Scratch

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

This project features a from-scratch implementation of the **Affinity Propagation (AP)** clustering algorithm in Python. The algorithm's performance is tested on various synthetic datasets designed to challenge clustering methods with different cluster shapes. The results are then compared against popular library implementations of K-Means and HDBSCAN.

---

## 📋 Project Overview

Affinity Propagation is a powerful clustering algorithm that does not require the number of clusters to be specified beforehand. This project demonstrates its implementation and capabilities through the following workflow:

1.  **Data Synthesis:**
    * Three distinct 2D datasets were generated using scikit-learn to test the algorithm under different conditions:
        * `make_circles`: For concentric, non-convex clusters.
        * `make_moons`: For interleaved, crescent-shaped clusters.
        * `make_blobs`: For standard, convex (Gaussian) clusters.

2.  **Algorithm Implementation:**
    * The Affinity Propagation algorithm was implemented **from scratch** using NumPy.
    * The core logic is based on the concept of "message-passing" between data points to determine which points are best suited to be cluster exemplars (centers).

3.  **Hyperparameter Selection & Evaluation:**
    * Selected and justified appropriate hyperparameters for the AP algorithm.
    * Applied the implemented algorithm to all three synthetic datasets and visualized the resulting clusters.
    * Evaluated the quality of the clusters using internal validation metrics suitable for unsupervised learning tasks.

4.  **Comparative Analysis:**
    * To benchmark the from-scratch AP implementation, the same datasets were clustered using library versions of **K-Means** and **HDBSCAN**.
    * The results were compared to analyze the relative strengths and weaknesses of each algorithm on different data structures.

---

## 🛠️ Technologies Used
* Python
* NumPy
* scikit-learn (for data generation and comparison algorithms)
* Matplotlib / Seaborn
* Jupyter Notebook

---

## 🚀 Usage

1.  **Clone the repository:**
    ```bash
    git clone <your-repository-url>
    cd <repository-name>
    ```
2.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
3.  **Run the analysis:**
    Open and run the cells in the `code.ipynb` Jupyter Notebook to execute the entire pipeline, from data generation to final evaluation and comparison.

---

## 📄 License
This project is licensed under the MIT License.