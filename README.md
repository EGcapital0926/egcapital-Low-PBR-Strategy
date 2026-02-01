# Low PBR Strategy

Quantitative value investment strategy exploiting the Price-to-Book Ratio anomaly in Japanese equities (TSE).

## Performance Summary (Feb 2017 - Dec 2025)

- **Total Return**: 327.10%
- **Sharpe Ratio**: 1.32
- **Information Ratio**: 0.26
- **Max Drawdown**: -27.14%

## Quick Start

### Prerequisites
```bash
pip install pandas numpy scipy matplotlib seaborn jupyter
```

### Data Requirements

⚠️ **Raw data not included** (J-Quants API terms of service).

Required data structure:
```
EGCapital/JE/
├── data/raw/              # Place J-Quants data here
│   ├── stock_prices/
│   ├── financials/
│   ├── master/
│   └── indices/
└── Research/PBR/          # This repository
    └── Low_pbr_strategy.ipynb
```

Get data from: https://jpx-jquants.com/

### Run
```bash
jupyter notebook Low_pbr_strategy.ipynb
```

## Repository Structure
```
├── Low_pbr_strategy.ipynb    # Main analysis
├── processed/                 # Portfolio data
└── outputs/                   # Figures & reports
```

## Methodology

- **Universe**: Top 300 TSE stocks by float-adjusted market cap
- **Selection**: 10 lowest PBR stocks (equal-weighted)
- **Rebalancing**: Monthly

Full methodology and findings are documented in the notebook.

## License

MIT License