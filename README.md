
# Statistical Analysis of Kaggle Classification Dataset

This project presents a comprehensive statistical analysis of the Kaggle classification dataset, examining various relationships, hypothesis tests, and visualizations across different variables. The analysis covers multiple aspects of the dataset, including both categorical and numerical features, and performs hypothesis testing to draw meaningful insights.

## Table of Contents

- [Overview](#overview)
- [Data Exploration](#data-exploration)
- [Hypothesis Testing](#hypothesis-testing)
  - [1. Admission Grade vs Target](#admission-grade-vs-target)
  - [2. Marital Status vs Target](#marital-status-vs-target)
  - [3. GDP vs Unemployment Rate](#gdp-vs-unemployment-rate)
  - [4. GDP vs Inflation Rate](#gdp-vs-inflation-rate)
- [Correlation Analysis](#correlation-analysis)
- [Conclusion](#conclusion)

## Overview

This analysis aims to uncover significant patterns in the dataset related to various features such as Admission grade, Marital status, GDP, and Unemployment rate. By employing statistical methods like One-way ANOVA and Chi-square tests, we draw insights into relationships between categorical and numerical variables.

The dataset contains different features, some of which are continuous (e.g., GDP, Unemployment rate), and some are categorical (e.g., Gender, Marital status). We utilize data visualization techniques to better understand the distribution and associations of these variables.

## Data Exploration

### Data Overview

The dataset contains multiple features including both categorical and numerical data. We start by reviewing the general statistics and the distribution of each feature.

```python
df.info()
df.describe(include='all')

# Hypothesis Testing

1. Admission Grade vs Target
Hypothesis

H0: There is no significant difference in the means of the "Admission grade" across different "Target" groups.
H1: At least one "Target" group mean is significantly different from the others.
Using One-way ANOVA, we found a significant difference in the "Admission grade" across "Target" groups.

f_stat, p_value = f_oneway(graduate, dropout, enrolled)
