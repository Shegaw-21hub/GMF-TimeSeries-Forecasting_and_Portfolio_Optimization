# GMF Investments: Time Series Forecasting and Portfolio Optimization

## 📖 Project Overview

This project is an **end-to-end financial analysis pipeline** developed for **Guide Me in Finance (GMF) Investments**.  
The primary objective is to enhance personalized portfolio management by leveraging data-driven insights from **time series forecasting** and **Modern Portfolio Theory (MPT)**.

The final goal is to develop a robust strategy for:

- 📈 Predicting market trends  
- ⚖️ Optimizing asset allocation  
- 🔁 Validating performance through backtesting

---

So far, we have successfully completed **Task 1: Data Exploration and Preprocessing**, which included:

- ⚙️ Setting up a **reproducible data pipeline**
- 🧹 Cleaning raw market data for key assets: **TSLA**, **BND**, and **SPY**
- 📊 Conducting an in-depth **exploratory data analysis** to understand their **risk** and **return** characteristics
## 📂 Folder Structure

The project is organized into a modular and easy-to-navigate directory structure:

### 📓 notebooks/
Contains the Jupyter notebooks for interactive development and analysis:

- **EDA.ipynb**: The notebook for the completed Task 1, covering data loading, cleaning, and exploratory analysis.  
- **Forecasting.ipynb**: Will house the code for Task 2 (time series modeling).  
- **Portfolio_Optimization.ipynb**: Will contain the code for Tasks 3, 4, and 5 (forecasting, MPT, and backtesting).

### 🧠 src/
Stores all reusable Python scripts and functions for a clean, modular codebase:

- **data_loader.py**: Handles data fetching and initial preprocessing.  
- **eda.py**: Contains functions for data visualization and statistical analysis.  
- **models.py**: Will contain functions for building and evaluating forecasting models.  
- **portfolio.py**: Will contain functions for portfolio optimization.  
- **backtest.py**: Will contain functions for backtesting the final strategy.

### 📁 data/
Stores the project's data files:

- **raw/**: Contains the initial raw data downloaded from YFinance.  
- **processed/**: Contains cleaned and preprocessed data, ready for modeling.

### 🖼️ images/
Stores all generated plots and visualizations.

### 📄 requirements.txt  
Lists all necessary Python dependencies.
## 🛠️ Setup & Execution

### 1. Environment Setup

1. **Clone the repository and navigate to the project directory:**

   ```bash
   git clone https://github.com/Shegaw-21hub/GMF-TimeSeries-Forecasting_and_Portfolio_Optimization
   cd GMF-TimeSeries-Forecasting_and_Portfolio_Optimization
2. **Create and activate a Python virtual environment:**

   ```bash
   python -m venv venv
   .\venv\Scripts\activate       # For Windows
   # source venv/bin/activate    # For macOS/Linux
3. **Install all required libraries from `requirements.txt`:**

   ```bash
   pip install -r requirements.txt
2. Running the Code  
Launch Jupyter Notebook:  
  ```bash
  ➡️jupyter notebook
  ```
    ➡️ **Open the** `notebooks/EDA.ipynb` **file and execute  all cells sequentially to reproduce the data preprocessing and exploratory analysis for** ***Task 1***.
## 📈 Key Insights & Preliminary Results (Task 1)

The initial analysis of **TSLA**, **BND**, and **SPY** data from **July 2015 to July 2025** yielded critical insights.
- **Data Quality:**  
  The YFinance data was complete, and our preprocessing pipeline successfully handled column formatting and potential missing values.

- **Stationarity:**  
  The raw price series for all assets were non-stationary (ADF p-values > 0.05), confirming the need for differencing before using models like ARIMA.  
  In contrast, the daily returns were stationary (ADF p-values ≈ 0.00), making them suitable for modeling.
- **Risk & Return:**

  - **TSLA** is a high-risk, high-reward asset with a CAGR of **33.04%** and an annualized volatility of ~**59%**.

  - **SPY** offers diversified, moderate exposure with an annualized volatility of ~**18%**.

  - **BND** provides stability with very low volatility (~**5%**) but also a very low historical Sharpe Ratio.

- **Risk Metrics:**  
  The 95% daily Value at Risk (VaR) was highest for **TSLA** (**5.47%**), followed by **SPY** (**1.72%**) and **BND** (**0.49%**).  
  This quantifies the potential daily loss on 95% of trading days.
## 🚀 Future Work Roadmap

The project is on track to complete the remaining tasks in the following order:

- **Task 2: Develop Forecasting Models:**  
  Build and compare an ARIMA/SARIMA model with an LSTM model to predict TSLA's future stock prices.

- **Task 3: Forecast Future Market Trends:**  
  Use the best-performing model to generate a 6-12 month forecast for TSLA, including confidence intervals.

- **Task 4: Optimize Portfolio:**  
  Apply the TSLA forecast alongside historical data for BND and SPY to generate the Efficient Frontier and identify optimal portfolios.

- **Task 5: Strategy Backtesting:**  
  Simulate the performance of the chosen portfolio against a benchmark to validate the strategy.
## 📬 Contact Information

**Shegaw Adugna Melaku**  
📧 Email: [Send me an email](mailto:shegamihret@gmail.com)  
🔗 LinkedIn: [Visit my LinkedIn profile](https://www.linkedin.com/in/shegaw-adugna-b751a1166/)

---

*Feel free to reach out for collaborations, questions, or just to connect! 🚀*
