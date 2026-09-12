# Portfolio Optimization

**Author:** Nazmi Syed · B.S.–M.S. Exploration Geophysics, IIT Kharagpur

This project performs portfolio optimization aimed at maximizing the Sharpe Ratio using historical stock data. It leverages Modern Portfolio Theory (MPT) to identify the optimal asset allocation and employs Monte Carlo simulations to estimate Value at Risk (VaR).

## Features

- **Data Retrieval**: Fetches historical stock data (Adjusted Close prices) using `yfinance`.
- **Financial Metrics**: Calculates daily log returns, covariance matrix, expected returns, and standard deviation (volatility).
- **Portfolio Optimization**:
  - Maximizes the Sharpe Ratio using `scipy.optimize.minimize`.
  - Determines optimal weights for the selected assets.
- **Efficient Frontier**: Analysis of risk vs. return trade-offs.
- **Value at Risk (VaR)**:
  - Calculates VaR using parametric methods.
  - Performs Monte Carlo simulations to estimate VaR at a 95% confidence level.
  - Visualizes the distribution of daily VaR.

## Files

- **`Portfolio_Opt.ipynb`**: The main notebook containing the portfolio optimization logic, including data fetching, optimization, and VaR calculation using Monte Carlo simulations.
- **`VaR.ipynb`**: A notebook focused on Value at Risk calculation, likely for single asset analysis or testing (requires `Data.csv`).
- **`README.md`**: This project documentation.

## Technologies Used

- **Python**: Primary programming language.
- **yfinance**: For downloading historical market data.
- **Pandas**: For data manipulation and analysis.
- **NumPy**: For numerical computations.
- **Matplotlib**: For data visualization.
- **SciPy**: For optimization algorithms.

## Usage

1.  **Install Dependencies**:
    Ensure you have the required libraries installed:
    ```bash
    pip install yfinance pandas numpy matplotlib scipy
    ```

2.  **Run the Notebook**:
    Open `Portfolio_Opt.ipynb` in Jupyter Notebook or Google Colab and run the cells sequentially to see the analysis and results.

3.  **Customization**:
    - Modify the `tickers` list in `Portfolio_Opt.ipynb` to analyze different stocks.
    - Adjust the `start_date` and `end_date` to change the time period.
