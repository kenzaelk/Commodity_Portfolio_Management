# Commodity_Portfolio_Management

This repository focuses on portfolio management for commodities using historical price data. It includes forecasting and performance analysis models aimed at optimizing commodity portfolios. The project utilizes machine learning techniques to predict commodity prices and analyze portfolio returns, incorporating various strategies for risk management and optimization.

## Project Overview

The main objective of this project is to design and evaluate RL models that learn to optimize the allocation of a commodity portfolio by maximizing returns while managing risks. The project includes:
- **Data Preprocessing:** Historical returns data for commodities is processed, normalized, and clustered using PCA (Principal Component Analysis) and KMeans clustering.
- **LSTM Forecasting:** LSTM forecasting is incorporated to predict future returns and provide a more accurate decision-making process.
- **Reinforcement Learning Models:** The PPO and TD3 models are trained and evaluated for portfolio optimization.
- **Performance Metrics:** Several risk-adjusted performance metrics (such as Conditional Value at Risk - CVaR, Return-to-Risk Ratio - R2R, and volatility) are computed and visualized.
- **PPO-LSTM Integration:** An extension of the PPO model with an LSTM feature extractor is implemented to capture temporal dependencies in the return series.

## Repository Structure

- `commodities_DAILY.csv`: A dataset of daily commodity price data. This file is the core dataset used for analysis and model training.
- `forecasting-performance.ipynb`: Jupyter notebook dedicated to forecasting the portfolio performance using machine learning models.
- `portfolio-performance.ipynb`: Jupyter notebook containing the complete portfolio performance analysis.

## Getting Started


### Prerequisites

- Python 3.8 or higher
- Jupyter Notebook

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/Commodity_Portfolio_Management.git
    cd Commodity_Portfolio_Management
    ```

2. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

### Usage

1. Open the Jupyter notebooks in the repository using Jupyter Notebook or Jupyter Lab:
    ```bash
    jupyter notebook
    ```

2. Navigate to the desired notebook (`forecasting-performance.ipynb` or `portfolio-performance.ipynb`) and run the cells to perform data analysis and model training.
3. 

## Methodology
### Data Preprocessing
- **Cleaning:** Handle missing values and outliers.
- **Feature Engineering:** Create new financial ratios and performance indicators.
- **Normalization:** Scale data for machine learning models.

### Performance Metrics
The following metrics are calculated to assess portfolio performance:

Value at Risk (VaR): Estimates the potential loss at a given confidence level.

Conditional Value at Risk (CVaR): Measures expected loss beyond VaR.

### Machine Learning Models

The forecasting of portfolio performance is done using Long Short-Term Memory (LSTM) models. LSTM is a type of recurrent neural network (RNN) well-suited for time series data like financial returns, allowing the model to capture long-term dependencies in historical data for accurate forecasting.

Forecasting Portfolio Performance
The forecasting-performance.ipynb focuses on using machine learning models to forecast the future performance of the portfolio based on historical data. It includes:

Feature Selection: Identifying relevant features that impact future performance.

Modeling: Training models to predict future returns and performance indicators.

Evaluation: Comparing forecast accuracy with real-world data to assess model robustness.

Visualization
Cumulative Returns: Compare portfolio growth over time.

Risk-Return Scatterplots: Show portfolio positioning relative to benchmarks.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or additions.
