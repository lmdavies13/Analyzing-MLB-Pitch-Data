# Analyzing MLB Pitch Data (2015-2018)
SUNY Brockport CSC435 Project - Data Analytics and Predictive Modeling

This repository contains code and Quarto documents for analyzing MLB pitch trends. Our goals are to:

- Understand pitching trends across MLB.
- Build models to classify pitch types.
- Predict pitch speeds based on various factors.

## Getting Started

### 1. Clone or download this repository

```bash
git clone https://github.com/lmdavies13/Analyzing-MLB-Pitch-Data.git
```

Open it in RStudio (or your preferred environment).

### 2. Acquire the dataset

We use the Kaggle MLB dataset (specifically the `pitches.csv` file).
https://www.kaggle.com/datasets/pschale/mlb-pitch-data-20152018/data

- Download `pitches.csv` from Kaggle.
- Place it in the root directory of this project.
- Note that `.gitignore` is configured to ignore `pitches.csv` so you won’t accidentally commit large data files.

## Usage

### 1. Open the Quarto document

- The main analysis file is `Analyzing MLB Pitch Trends.qmd`.
- You can view or modify code chunks, run them in RStudio, and see results interactively.

### 2. Render the Quarto document

If you’ve made updates and want to generate a new HTML report, run this command in your terminal (or the RStudio terminal pane):

```bash
quarto render 'Analyzing MLB Pitch Trends.qmd' --output-dir docs
```

This will compile the `.qmd` file into an HTML document in the `docs` folder.

### 3. View the HTML report

After rendering, an updated HTML file is placed in `docs/`. You can open it directly in your web browser to see the latest analysis.

- If you only want to read the existing report without re-rendering, just open the HTML file found in `docs/`.
