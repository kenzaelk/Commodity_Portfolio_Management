# Commodity_Portfolio_Management

This repository focuses on portfolio management for commodities using historical price data. It includes forecasting and performance analysis models aimed at optimizing commodity portfolios. The project utilizes machine learning techniques to predict commodity prices and analyze portfolio returns, incorporating various strategies for risk management and optimization.

## Project Overview

The main objective of this project is to design and evaluate RL models that learn to optimize the allocation of a commodity portfolio by maximizing returns while managing risks. The project includes:
- **Data Preprocessing:** Historical returns data for commodities is processed, normalized, and clustered using PCA (Principal Component Analysis) and KMeans clustering.
- **LSTM Forecasting:** LSTM forecasting is incorporated to predict future returns and provide a more accurate decision-making process.
- **Reinforcement Learning Models:** The PPO and TD3 models are trained and evaluated for portfolio optimization.
- **Performance Metrics:** Several risk-adjusted performance metrics (such as Conditional Value at Risk - CVaR, Return-to-Risk Ratio - R2R, and volatility) are computed and visualized.
- **Hybrid PPO-LSTM Model Integration:** Combines reinforcement learning (PPO) with deep learning (LSTM) to improve predictions and decision-making.

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

## Methodology
### Data Preprocessing
- **Feature Engineering:** Extracts key financial indicators to enhance predictive accuracy.
- **Market Regime Detection:** Uses clustering techniques to classify different market conditions.
- **Normalization:** Scales data to ensure consistent model performance.

### Proposed Model Architecture
# Proximal Policy Optimization (PPO) + LSTM
- PPO helps optimize trading strategies using a policy-gradient approach.
- LSTM captures long-term dependencies in commodity price movements.
- The combined PPO-LSTM framework improves decision-making adaptability.

### Performance Metrics
To assess the effectiveness of the models, the following key metrics are used:

- **Annual Volatility Analysis:** Measures the risk associated with different trading strategies.
- **Cumulative Return Comparison:** Evaluates overall profitability against baseline models.
- **Reward to Risk (R2R):** Determines the trade-off between risk and return for each model.
- **Conditional Value at Risk (CVaR):** Estimates potential losses in extreme market conditions, ensuring robust risk management.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or additions.
