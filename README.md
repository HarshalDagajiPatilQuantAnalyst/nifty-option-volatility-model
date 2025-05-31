# Nifty Option Volatility Model

This project estimates the **Implied Volatility (IV)** of **Nifty options** using both the **Black-Scholes** and **SABR** models. It builds a **volatility smile** by calculating implied volatilities across various strike prices for a fixed expiry and visualizes the results. The project begins with an Excel implementation and extends to Python.

---

## Objective

To construct a **volatility smile** and analyze how market IV compares with model-generated IV:
- Compute implied volatilities using market option prices.
- Apply both Black-Scholes and SABR models to estimate IV.
- Plot and compare model vs. market implied volatilities.

---

## Data Columns

- `Date`, `Expiry`, `DTE` (Days to Expiry)  
- `Spot`, `Strike`  
- `Option Type` (Call or Put)  
- `Market Price` (Mid of Bid-Ask Spread)  
- `Risk-free Rate`

### Computed Columns

- `d1`, `d2` (Intermediate terms in BS formula)  
- `IV(%)` – Market Implied Volatility  
- `IV_BS` – Black-Scholes Implied Volatility  
- `IV_SABR` – SABR Model Implied Volatility

---

## Methods Used

- **Black-Scholes Pricing Model**
  - Analytical pricing for European options
  - Goal Seek (Excel) and `scipy.optimize` (Python) to derive IV
- **SABR Model**
  - Calibrated to fit IV smile/skew
  - Captures volatility dynamics better than BS
- **Visualization**
  - `matplotlib` and `seaborn` for plotting IV vs. Strike

---

## Files


