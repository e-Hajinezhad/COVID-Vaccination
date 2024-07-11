# COVID Vaccination Modeling

This project presents the methodology and results of modeling COVID vaccination prediction using two regression techniques: Prophet and Polynomial Regression.

## Table of Contents

1. [Project Overview](#project-overview)
2. [Data Preparation](#data-preparation)
3. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
4. [Preprocessing](#preprocessing)
5. [Regressor Modeling](#regressor-modeling)
6. [Model Evaluation](#model-evaluation)
7. [Model Selection](#model-selection)
8. [Getting Started](#getting-started)
9. [Dependencies](#dependencies)
10. [Usage](#usage)
11. [Contributing](#contributing)
12. [License](#license)

## Project Overview

This project aims to predict COVID vaccination trends using two regression techniques and compare their performances. The dataset used includes various vaccination-related metrics from different countries.

## Data Preparation

- Essential libraries are imported to facilitate data analysis and modeling.
  - `numpy`
  - `pandas`
  - `matplotlib`
  - `seaborn`
  - `sklearn`
  - `prophet`
- The vaccination dataset is imported for analysis.

## Exploratory Data Analysis (EDA)

- Initial exploratory analysis revealed that columns such as `iso_code`, `source_name`, and `source_website` were not pertinent for prediction modeling and were subsequently removed.
- For further analysis, the `vaccine` column is expanded into separate columns representing different vaccine types.
- Trends in total vaccination for two countries, Iran and USA, are illustrated.
- The distribution of vaccines across countries indicates that "Oxford/AstraZeneca" is the most widely used.

## Preprocessing

- NaN values are handled by interpolation, with entries containing few NaNs being dropped.
- Three columns with excessive NaN values (`total_vaccinations_per_hundred`, `people_vaccinated_per_hundred`, `people_fully_vaccinated_per_hundred`) are removed.

## Regressor Modeling

- Prophet and Polynomial Regression are applied to the dataset. 

## Model Evaluation

- Model performance is assessed using mean absolute percentage error and R-squared error metrics.

## Model Selection

- While Prophet achieved a 0.95 R-squared, the Polynomial Regression performed significantly better, with a 0.99 R_squared.

## Getting Started

To get a copy of this project up and running on your local machine, follow these steps.

### Prerequisites

Ensure you have Python installed on your machine. You can download it from [python.org](https://www.python.org/).

### Installation

Clone the repository:

git clone https://github.com/e-Hajinezhad/COVID-Vaccination.git
