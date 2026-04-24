# Experiment 18: Advanced Data Visualization Using Matplotlib and Seaborn

**Name:** Arhan Nair  
**PRN:** 25070123169  


---

## 1. Theory

### Advanced Statistical Visualization
Beyond basic charts, advanced data visualization focuses on understanding the distribution, density, and relationships within a dataset simultaneously. Tools like Seaborn offer high-level functions to visualize complex statistical relationships with minimal code, allowing for deeper exploratory data analysis (EDA).

### Key Advanced Plot Types
The following specialized visualizations were implemented in this experiment:
* **Violin Plot**: Combines a box plot with a kernel density plot. It shows the distribution of data across different levels of one or more categorical variables, allowing for a comparison of the probability density of the data.
* **Heatmap**: A graphical representation of data where individual values contained in a matrix are represented as colors. It is predominantly used to visualize **correlation matrices** to identify the strength of relationships between all numeric variables in a dataset.
* **Pair Plot**: Creates a grid of scatter plots for every pair of features in a dataset. It is an essential tool for identifying multi-dimensional patterns and correlations at a single glance.

---

## 2. Implementation Overview

### Academic and E-commerce Datasets
The experiment applied advanced plotting techniques to the student performance and order datasets.

* **Violin Plot Implementation**: Used to visualize the distribution of "Marks" across different "Departments". This revealed not just the median and quartiles, but also the specific peaks in grade density for each department.
* **Heatmap and Correlation**: 
    * Calculated the correlation matrix for numeric features such as **Price**, **MPG.city**, and **Horsepower** from the `Cars93` dataset.
    * Plotted the matrix using `sns.heatmap()` with `annot=True` to display the exact correlation coefficients.
* **Pair Plot Analysis**: Generated a pair plot for the `Cars93` dataset to observe how physical attributes like **Horsepower** interact with performance metrics like **MPG.city** across the entire sample.

---

## 3. Conclusion

This experiment demonstrates that advanced visualization techniques provide a more comprehensive view of data than basic charts. By using heatmaps and pair plots, we can immediately identify which features are redundant and which are strongly correlated, which is a vital step in feature selection for machine learning.

**Key Takeaways:**
* **Density Insights**: Violin plots provide a superior understanding of data "clumping" compared to standard box plots.
* **Relationship Discovery**: Heatmaps simplify the identification of multicollinearity (high correlation between independent variables), helping to refine model inputs.
* **Multi-dimensional Exploration**: Pair plots serve as the ultimate "first look" tool for a new dataset, highlighting clusters and linear relationships across all variables simultaneously.
* **Aesthetic and Functional Balance**: Using Seaborn's built-in themes (e.g., `sns.set_theme()`) ensures that complex plots remain readable and professional for reporting.

---
