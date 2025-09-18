# WARP.md

This file provides guidance to WARP (warp.dev) when working with code in this repository.

## Overview

This repository contains machine learning educational notebooks focused on data analysis fundamentals. The codebase consists of three Jupyter notebooks that demonstrate different aspects of exploratory data analysis using Python data science libraries.

## Code Architecture

### Structure
The repository is organized as a collection of educational notebooks:

- `understanding_data.ipynb` - Foundation notebook covering essential data exploration questions
- `Univariate_Analysis.ipynb` - Analysis of single variables/columns in datasets
- `Bi_Multivariate_Analysis.ipynb` - Analysis of relationships between multiple variables

### Data Pipeline
The notebooks follow a structured approach to data analysis:

1. **Data Loading** - Using pandas to read CSV files
2. **Data Understanding** - Systematic exploration of dataset characteristics
3. **Visualization** - Using seaborn and matplotlib for data visualization
4. **Analysis** - Statistical analysis including correlation analysis

### Key Libraries Used
- `pandas` - Data manipulation and analysis
- `seaborn` - Statistical data visualization
- `matplotlib.pyplot` - Basic plotting functionality

## Common Development Tasks

### Running Notebooks
These are Jupyter notebooks that should be run in an environment with the following dependencies installed:
```bash
pip install pandas seaborn matplotlib
```

### Data Requirements
The notebooks expect a `train.csv` file in the root directory. This appears to be the Titanic dataset based on the column structure (PassengerId, Survived, Pclass, Name, Sex, Age, SibSp, Parch, Ticket, Fare, Cabin, Embarked).

### Visualization Patterns
The codebase demonstrates several visualization patterns:
- Scatter plots for numerical-numerical relationships
- Bar plots for categorical data
- Box plots for numerical-categorical relationships
- Count plots for categorical distributions
- Histograms for numerical distributions
- Pie charts for proportion visualization

### Data Analysis Framework
Each notebook follows a systematic approach to data analysis:
1. **Size assessment** - Understanding dataset dimensions
2. **Data inspection** - Examining sample data and data types
3. **Missing value analysis** - Identifying incomplete data
4. **Duplicate detection** - Ensuring data quality
5. **Statistical summary** - Understanding data distributions
6. **Correlation analysis** - Identifying relationships between variables

## Best Practices

When working with this codebase:
- Use `data.sample()` instead of `data.head()` for better data inspection
- Include both numerical and visual analysis for comprehensive understanding
- Consider missing value patterns when interpreting results
- Use appropriate visualization types for different data relationships

## Environment Setup

Ensure you have a Jupyter notebook environment set up with the required dependencies. The notebooks are designed to work with Google Colab as evidenced by the output metadata.