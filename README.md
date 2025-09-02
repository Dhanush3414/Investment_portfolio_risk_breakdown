# Investment Portfolio Risk Breakdown

![Python](https://img.shields.io/badge/Python-3.7%2B-blue)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange)
![Google Colab](https://img.shields.io/badge/Google-Colab-green)

A comprehensive **Exploratory Data Analysis (EDA)** project that dissects and visualizes the various facets of investment risk in a stock portfolio. This analysis transforms raw historical stock data into actionable insights, providing a clear visual breakdown of risks associated with different investment strategies.

## Objectives

- **Time-Series Analysis:** Visualize the performance of individual stocks and a sample portfolio over a 5-year period.
- **Risk Measurement:** Calculate and compare key risk metrics, primarily volatility (standard deviation of returns).
- **Correlation Analysis:** Evaluate portfolio diversification by visualizing the correlation between asset returns.
- **Anomaly Detection:** Identify periods of extreme volatility and anomalous returns using statistical methods.
- **Dimensionality Reduction:** Use Principal Component Analysis (PCA) to visualize stock clusters based on their return profiles.

## Dataset

The project uses the **"5-Year Stock Data"** dataset, which contains the daily OHLCV (Open, High, Low, Close, Volume) data for all S&P 500 companies from 2013 to 2018.

- **Source:** [Kaggle - 5 Years Historical Stock Prices](https://www.kaggle.com/datasets)
- **Rows:** ~619,040
- **Columns:** `date`, `open`, `high`, `low`, `close`, `volume`, `Name` (Ticker Symbol)

## Installation & Setup

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/investment-portfolio-risk-breakdown.git
    cd investment-portfolio-risk-breakdown
    ```

2.  **Create a virtual environment (recommended):**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```

3.  **Install the required dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Launch Jupyter Notebook:**
    ```bash
    jupyter notebook
    ```
    Open and run the `Investment_Portfolio_Risk_Breakdown.ipynb` notebook.

## Requirements

All required Python libraries are listed in `requirements.txt`. The main libraries include:
- pandas & numpy for data manipulation
- plotly & matplotlib for interactive visualizations
- seaborn for statistical graphics
- scikit-learn for PCA and standardization
- ipywidgets for interactive controls

## Key Features

- **Interactive Portfolio Dashboard:** Widgets to select stocks and adjust moving average windows.
- **Dynamic Visualizations:** Interactive Plotly charts for deep exploration (zooming, panning, hover details).
- **Correlation Heatmaps:** Visualize how asset returns move together to assess diversification.
- **Risk-Return Scatter Plot:** Plot stocks based on their annualized return vs. volatility.
- **PCA Biplot:** Reduce dimensionality to visualize clusters of stocks with similar return profiles.

## Results and Insights

The analysis provides clear insights into:
- The relative risk (volatility) and performance of major stocks like AAPL, AMZN, and GOOGL.
- The diversification benefits (or lack thereof) within a portfolio of tech-heavy stocks.
- Historical periods of high market stress and volatility.
- How different assets contribute to overall portfolio risk.

## Usage

1.  Run the Jupyter notebook cells sequentially to load data, perform calculations, and generate visualizations.
2.  Use the dropdown menu to select a specific stock for focused analysis.
3.  Adjust the "MA Days" slider to change the window for the moving average line, helping to identify trends.
4.  Explore the various tabs and visualizations to understand different aspects of portfolio risk.

## Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/your-username/investment-portfolio-risk-breakdown/issues).

## Acknowledgments

- Dataset provided by Kaggle.
- Built with amazing open-source libraries like Pandas, Plotly, and Scikit-learn.
