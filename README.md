# Data Visualization in R

This repository contains a comprehensive data visualization project analyzing the **Abalone dataset** using R. The project demonstrates various visualization techniques including pair plots, box plots, sina plots, PCA analysis, and interactive visualizations using Plotly.

## Project Overview

This project focuses on exploring and visualizing the Abalone dataset to understand the relationships between physical measurements and age (represented by rings). The analysis includes:

- **Exploratory Data Analysis (EDA)** using pair plots
- **Distribution Analysis** with box plots and sina plots
- **Dimensionality Reduction** using Principal Component Analysis (PCA)
- **Explanatory Visualizations** showing relationships between length and height
- **Interactive Visualizations** using Plotly for dynamic exploration

## Dataset

### About the Abalone Dataset

The Abalone dataset is used to predict the age of abalones based on physical measurements. The dataset contains:

- **4,177 instances** with 8 features and 1 target variable
- **Features**: Sex, Length, Diameter, Height, Whole weight, Shucked weight, Viscera weight, Shell weight
- **Target**: Rings (age = rings + 1.5)

### Methodology

According to the dataset documentation:
> "The age of abalone is determined by cutting the shell through the cone, staining it, and counting the number of rings through a microscope."

The dataset has been preprocessed with missing values removed.

## Visualizations

### 1. Pair Plot
- Comprehensive pairwise relationships between all features
- Color-coded by sex (Female, Male, Infant)
- Shows correlations and density distributions

### 2. Box and Sina Plots
- Distribution of features across different ring (age) categories
- Rings categorized into groups: 0-5, 6-10, 11-15, 16-20, 21-25
- Combines box plots with sina plots for detailed distribution view

### 3. PCA Analysis
- Reduces dimensionality to visualize patterns
- First two principal components explain most variance
- Faceted by sex to show group differences

### 4. Length vs Height Analysis
- Scatter plots with linear regression lines
- Faceted by sex
- Shows strong relationship between length and height

### 5. Interactive Plotly Visualization
- Interactive scatter plot with marginal histograms
- Hover functionality to explore individual data points
- Regression lines for each sex category
- Downloadable as PNG image

## Requirements

The project uses the following R packages:

```r
library(tidyverse)   # Data manipulation and visualization
library(ggplot2)     # Static plotting
library(GGally)      # Pair plots
library(ggforce)     # Sina plots
library(plotly)      # Interactive visualizations
library(RColorBrewer) # Color palettes
```

## Installation

To run this project, you need R installed on your system. Install the required packages:

```r
install.packages(c("tidyverse", "ggplot2", "GGally", "ggforce", "plotly", "RColorBrewer"))
```

## Usage

1. Clone this repository:
   ```bash
   git clone https://github.com/sacdart/Data-visualization-in-R.git
   cd Data-visualization-in-R
   ```

2. Open the R Markdown file:
   ```r
   # In R or RStudio
   rmarkdown::render("20956528_FinalProject-2.Rmd")
   ```

3. View the generated HTML output:
   - Open `20956528_FinalProject-2.html` in your web browser

## Key Findings

The analysis reveals several insights:

1. **Strong Correlations**: Length and diameter are highly correlated, nearly identical in their relationship with age
2. **Height as a Factor**: Height also plays an important role in predicting abalone age
3. **Logarithmic Relationships**: Box plots show logarithmic relationships between physical measurements and rings
4. **Sex Differences**: Different patterns emerge when data is separated by sex category

## License & Citations

This dataset is licensed under the [Creative Commons Attribution 4.0 International (CC BY 4.0) license](https://creativecommons.org/licenses/by/4.0/).

### License Terms:
- **Sharing**: You can copy and redistribute the material in any medium or format
- **Adaptation**: You can remix, transform, and build upon the material for any purpose, including commercial use
- **Attribution**: You must give appropriate credit to the original authors

## Declaration

This project involved the use of generative AI for:
- Code commenting and documentation
- Figure debugging and graphics formatting
- Grammar improvements in documentation

## Author

**Yuet Shan LO**

## Repository Structure

```
.
├── README.md                           # This file
├── 20956528_FinalProject-2.Rmd        # Main R Markdown analysis file
├── 20956528_FinalProject-2.html       # Rendered HTML output
└── Data/
    ├── abalone-2.data                 # Abalone dataset
    └── abalone-2.names                # Dataset documentation
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## Acknowledgments

- Original Abalone dataset providers
- R community for excellent visualization packages
- Contributors to tidyverse, ggplot2, and plotly
