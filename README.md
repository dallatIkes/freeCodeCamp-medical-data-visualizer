# Medical Data Visualizer

This project is my solution to the **FreeCodeCamp "Medical Data Visualizer" challenge**. It analyzes medical examination data and visualizes it using categorical plots and heatmaps. It uses Python libraries: Pandas, Seaborn, Matplotlib, and NumPy.

## Project Overview

The project provides two main functions:

### 1. draw_cat_plot()
- Converts features into categorical data.
- Uses `pd.melt` to transform the DataFrame into long format.
- Counts occurrences of each value for features like cholesterol, gluc, smoke, alco, active, and overweight.
- Creates a categorical bar plot with Seaborn (`sns.catplot`) showing distributions split by cardio.
- Saves the plot as `catplot.png`.

### 2. draw_heat_map()
- Cleans the dataset by removing inconsistent blood pressure readings and extreme height/weight values.
- Computes the correlation matrix of all numerical features.
- Generates a heatmap with Seaborn (`sns.heatmap`), masking the upper triangle.
- Saves the plot as `heatmap.png`.

## Files

- `medical_examination.csv` - the dataset used.
- `main.py` - script to run the visualization functions.
- `test_module.py` - automated tests for both functions.
- `requirements.txt` - Python dependencies.

## How to Run

1. Install dependencies:

```
pip install -r requirements.txt
```

2. Run the main script:

```
python main.py
```

3. The plots will be saved in the current folder:
- `catplot.png`
- `heatmap.png`

## Notes

- `draw_cat_plot` ensures categorical features are ordered correctly for visualization.
- `draw_heat_map` filters out outliers to generate a clear correlation matrix.
- This project was completed as part of FreeCodeCamp's Data Analysis with Python certification.
