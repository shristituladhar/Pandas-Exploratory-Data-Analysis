# Exploratory Data Analysis - Roller Coasters

An exploratory data analysis (EDA) project using Python, Pandas, and Seaborn to clean and analyze a roller coaster dataset.

## Tech Stack

* **Python**
* **Pandas** (Data manipulation and cleaning)
* **Seaborn & Matplotlib** (Data visualization)
* **Jupyter Notebook**

## Project Workflow

### 1. Data Cleaning & Preparation
* Handled missing height values by combining the `height_value` and `height_ft` columns.
* Removed duplicate records based on `Coaster_Name` and `Location`.
* Reset DataFrame indices and checked for missing values across columns.

### 2. Univariate Analysis
* Plotted the top 10 introduction years for roller coasters using bar charts.
* Examined the distribution of `Speed_mph` using histograms and Kernel Density Estimation (KDE) curves.

### 3. Multivariate Analysis
* Created scatter plots to compare `Height_ft` and `Speed_mph`, categorized by coaster type and introduction year.
* Used `sns.pairplot` to inspect relationships across multiple numeric features.
* Generated an annotated correlation heatmap for numerical data.

### 4. Custom Question Analysis
* Filtered locations with a minimum of 10 rides to find which parks have the fastest average roller coaster speeds, visualized using a horizontal bar chart.

## Repository Contents

* `Pandas_EDA_Roller_Coasters.ipynb`: The Jupyter Notebook containing the code and outputs.
* `coaster_db.csv`: The dataset file.

## How to Run

1. Clone the repository.
2. Open the notebook in Jupyter Notebook, Jupyter Lab, or Google Colab.
3. Run the cells from top to bottom.
