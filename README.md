# Commodity_Portfolio_Management

This repository focuses on portfolio management for commodities using historical price data. It includes forecasting and performance analysis models aimed at optimizing commodity portfolios. The project utilizes machine learning techniques to predict commodity prices and analyze portfolio returns, incorporating various strategies for risk management and optimization.

## Project Overview

The main objective of this project is to design and evaluate RL models that learn to optimize the allocation of a commodity portfolio by maximizing returns while managing risks. The project includes:
  Data Preprocessing: Historical returns data for commodities is processed, normalized, and clustered using PCA (Principal Component Analysis) and KMeans clustering.

LSTM Forecasting: LSTM forecasting is incorporated to predict future returns and provide a more accurate decision-making process.

Reinforcement Learning Models: The PPO and TD3 models are trained and evaluated for portfolio optimization.

Performance Metrics: Several risk-adjusted performance metrics (such as Conditional Value at Risk - CVaR, Return-to-Risk Ratio - R2R, and volatility) are computed and visualized.

PPO-LSTM Integration: An extension of the PPO model with an LSTM feature extractor is implemented to capture temporal dependencies in the return series.

## Repository Structure

- `commodities_DAILY.csv`: A dataset of daily commodity price data. This file is the core dataset used for analysis and model training.
- `forecasting-performance.ipynb`: Jupyter notebook for 
- `portfolio-performance.ipynb`: Jupyter notebook for

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


## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or additions.
