# Exploratory Data Analysis with Pandas

An end-to-end Exploratory Data Analysis (EDA) project built using **Python, Pandas, and Seaborn** to clean, transform, and analyze a global roller coaster dataset.

## Tech Stack

* **Language:** Python
* **Core Data Library:** Pandas (Data manipulation, method chaining, grouping, filtering)
* **Visualization:** Seaborn & Matplotlib
* **Environment:** Jupyter Notebook

## Project Workflow & Steps

### 1. Data Cleaning & Preparation

* Dropped duplicate records using subset matching (`Coaster_Name`, `Location`, `Opening_Date`) combined with bitwise negation (`~df.duplicated()`).
* Reset DataFrame indices cleanly using `.reset_index(drop=True)` to remove row gaps and discard old index artifacts.
* Checked missing values across all columns using `.isna().sum()`.

### 2. Univariate Analysis (Feature Understanding)

* **Bar Charts:** Counted and plotted the top 10 introduction years for roller coasters using `.value_counts()` and `.plot(kind='bar')`.
* **Histograms & KDE:** Evaluated the distribution of `Speed_mph` using binned histograms (`bins=20`) and smooth Kernel Density Estimation curves.

### 3. Multivariate Analysis & Feature Relationships

* Created scatter plots (`sns.scatterplot`) tracking the relationship between `Height_ft` and `Speed_mph`, adding visual dimensions for `Type_Main` (steel vs. wooden) and `Year_Introduced`.
* Generated a multi-variable grid using `sns.pairplot` to scan numeric interactions simultaneously.
* Calculated correlation coefficients (`.corr()`) for numerical features and visualized them using an annotated `sns.heatmap`.

### 4. Custom Question Analysis

Answered specific analytical queries using advanced Pandas method chaining (`query`, `groupby`, `agg`, `sort_values`):

* Discovered which locations hold the fastest average roller coaster speeds while filtering out small parks with a minimum threshold of 10 rides (`count >= 10`).
* Displayed the final rankings using horizontal bar charts (`barh`) to optimize label readability.

## Repository Contents

* `Pandas_EDA_Roller_Coasters.ipynb`: The main Jupyter Notebook containing all clean code cells and outputs.
* `coaster_db.csv`: The underlying dataset used for the pipeline.

## 🛠️ How to Run

1. Clone the repository to your local machine.
2. Open the Jupyter Notebook file in your preferred environment (Jupyter Lab, VS Code, or Google Colab).
3. Run the cells sequentially from top to bottom to execute the complete pipeline.
