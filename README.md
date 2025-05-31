# Nifty Option Volatility Model

This project uses the Black-Scholes model to estimate the implied volatility (IV) of Nifty options at various strike prices and maturities (1M, 3M, 6M). The project begins with an Excel implementation and may be extended to Python.

## Objective

To build a volatility smile by computing implied volatilities across strikes for a fixed expiry.

## Data Columns

- Date, Expiry, DTE
- Spot, Strike
- Option Type (Call or Put)
- Market Price (Mid)
- Risk-free rate
- Computed: `d1`, `d2`, `Option Price`, `Implied Volatility`

## Methods Used

- **Black-Scholes Pricing Model**
- Goal Seek in Excel to compute Implied Volatility


## Files

- `/excel-model/VolatilitySmile_30May_to_30June2025.xlsx`: Excel implementation
- `/screenshots/`: Image previews

## Next Steps

- Python implementation
- SABR model fitting
- Surface plot for IV vs. Strike vs. Maturity

## License

[MIT](LICENSE)

