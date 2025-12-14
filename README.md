# Global Well-being Cluster Analysis (Unsupervised Learning)

## Project Overview

The objective of this project is to apply unsupervised learning techniques, specifically **K-Means Clustering**, to segment countries based on multiple well-being factors derived from the World Happiness Report data. The analysis aims to discover distinct, naturally occurring 'well-being profiles,' which can be used to categorize nations based on their socio-economic and perceptual metrics. This methodology mirrors industrial applications such as customer segmentation and machinery fault classification.

## Methodology and Technical Execution

### Technologies Used

* **Language:** Python
* **Environment:** Jupyter Notebook / Google Colab
* **Core Libraries:** `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`

### Clustering Strategy

The **Elbow Method** was utilized to determine the optimal number of clusters ($K$) that minimizes the Sum of Squared Errors (SSE). This step is crucial for ensuring the resulting segmentation is both statistically robust and meaningfully interpretable.

The **K-Means Clustering** algorithm was then applied to partition the data into the determined number of groups.

## Analysis and Key Findings

The cluster analysis yields distinct well-being profiles, allowing for segmentation based on the chosen features (e.g., `GDP per Capita`, `Social Support`, `Life Expectancy`).

### Cluster Characterization

The final analysis involves plotting the data and characterizing each identified cluster. This process allows us to define and name the profiles based on their dominant characteristics:

* **High Well-being Profile:** Countries characterized by high scores across all metrics (e.g., high `GDP per Capita` and high `Trust in Government`).
* **Social Support Profile:** Countries characterized by strong `Social Support` and `Generosity` despite potentially lower scores in economic factors.

### Visual Validation

The final step is the visualization of the clusters using appropriate dimensionality reduction techniques or direct feature scatter plots, allowing for a clear visual representation of the segmentation boundaries and internal variance.

## Project Setup

To clone and execute this analysis locally, use the following commands. Ensure all required dependencies listed in `requirements.txt` are installed.

```bash
git clone [Your Repository URL Here]
cd World-Happiness-Clustering-Analysis-Python
pip install -r requirements.txt
jupyter notebook K_Clustering_World_Happiness\ (1).ipynb
