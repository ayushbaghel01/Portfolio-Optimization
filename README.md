Here's a template for a GitHub README file for the project, including a brief description of the Sharpe, Sortino, and Treynor ratios:

---

# Portfolio Optimization and Efficient Frontier Visualization

This project provides a Python-based implementation for simulating multiple portfolios, visualizing the efficient frontier, and plotting the Capital Market Line (CML). The code demonstrates how to optimize portfolios by finding the one with the maximum Sharpe ratio, which is where the CML tangentially touches the efficient frontier.

## Features
- **Portfolio Simulation**: Generates multiple portfolios with random weights.
- **Efficient Frontier Visualization**: Plots the expected returns against the volatility of portfolios.
- **Capital Market Line (CML)**: Displays the CML, showing the relationship between risk (volatility) and return, starting from a risk-free rate.
- **Tangency Point Identification**: Highlights the optimal portfolio with the highest Sharpe ratio.

## Ratios Explained

### Sharpe Ratio
The Sharpe Ratio measures the performance of an investment compared to a risk-free asset, after adjusting for its risk. It is calculated as:
\[ \text{Sharpe Ratio} = \frac{R_p - R_f}{\sigma_p} \]
Where:
- \( R_p \) = Expected portfolio return
- \( R_f \) = Risk-free rate
- \( \sigma_p \) = Standard deviation of portfolio returns (volatility)

### Sortino Ratio
The Sortino Ratio is a variation of the Sharpe Ratio that differentiates harmful volatility from total overall volatility by using the standard deviation of negative asset returns (downside deviation) instead of the total standard deviation of asset returns. It is calculated as:
\[ \text{Sortino Ratio} = \frac{R_p - R_f}{\text{Downside Deviation}} \]
Where:
- Downside Deviation considers only the returns that fall below a defined minimum acceptable return.

### Treynor Ratio
The Treynor Ratio, also known as the reward-to-volatility ratio, measures returns earned in excess of that which could have been earned on a riskless investment per each unit of market risk. It is calculated as:
\[ \text{Treynor Ratio} = \frac{R_p - R_f}{\beta_p} \]
Where:
- \( \beta_p \) = Beta of the portfolio, a measure of its sensitivity to market movements.

## How to Run
1. **Clone the Repository**
   ```
   git clone https://github.com/ayushbaghel01/portfolio-optimization.git
   cd portfolio-optimization
   ```

2. **Install Dependencies**
   ```
   pip install -r requirements.txt
   ```

3. **Run the Script**
   ```
   python portfolio_optimization.py
   ```

## Dependencies
- `numpy`
- `pandas`
- `matplotlib`
- `yfinance`
- `scipy`

Ensure that you have these libraries installed before running the script.

## Contributing
Contributions are welcome! Please submit a pull request or open an issue to discuss any changes.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments
This project utilizes the `yfinance` library to download historical stock data and `matplotlib` for plotting. Special thanks to the open-source community for their contributions to these libraries.

---

Feel free to customize this README file further based on your specific project details, such as including examples, screenshots, or additional sections.
