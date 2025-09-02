
## **Dimensionality Reduction: PCA, t-SNE, and UMAP**

In this repository, we explore how to implement two advanced dimensionality reduction algorithms, **t-SNE** and **UMAP**, on synthetic data and compare them with **PCA**.

We start by generating a **synthetic dataset of blobs** in a 3D feature space and visualize the data in an **interactive 3D plot**.

Then, we use all three algorithms to **project the blobs into two dimensions** and color them to see how well each algorithm **preserves structure**, such as the separation between blobs and their relative density.


## **Algorithms Comparison**

### **1. PCA (Principal Component Analysis)**

* **Speed:** Fastest algorithm, takes very little time.
* **Structure Preservation:** Maintains distances and densities between blobs accurately.
* **Overlaps:** Keeps overlaps realistic as in the original data.
* **Best Use Case:** When you need **fast, simple, and clear visualization**.


### **2. t-SNE (t-Distributed Stochastic Neighbor Embedding)**

* **Clusters:** Creates visually clear clusters, sometimes points may go to the "wrong" cluster.
* **Speed:** Slower than PCA, but faster than UMAP.
* **Overlaps:** Handles overlaps moderately well, but not perfectly.
* **Best Use Case:** **Clear visualization** for small to medium-sized datasets.


### **3. UMAP (Uniform Manifold Approximation and Projection)**

* **Clusters:** Preserves original connections between clusters better than t-SNE.
* **Speed:** Slowest algorithm among the three.
* **Overlaps:** Handles overlaps **realistically** while preserving structure.
* **Best Use Case:** When **data structure preservation** is more important than speed.


## **Summary Table**

| Algorithm | Speed   | Structure Preserve | Clusters Separation | Overlap Handling       | Best For                      |
| --------- | ------- | ------------------ | ------------------- | ---------------------- | ----------------------------- |
| **PCA**   | Fastest | Good               | Okay                | Realistic (Original)   | Simple, fast visualization    |
| **t-SNE** | Medium  | Medium             | Good Visual Clarity | Sometimes Wrong Points | Small datasets, clear visuals |
| **UMAP**  | Slowest | Best               | Balanced            | Realistic + Connected  | Structure preservation        |


## **Conclusion**

* **PCA** is best when speed and simplicity matter.
* **t-SNE** provides clearer clusters but may misplace some points.
* **UMAP** preserves the original structure better but takes more time.
* Advanced algorithms are not always better than simpler methods like PCA.
