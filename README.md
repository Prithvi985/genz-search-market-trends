# From Gen Z Interests to Market Trends: Predicting Emerging Consumer Demand

Foundations of Data Science, final project. Prithviraj Jhunjhunwala (2310110232) and Tanisha Agarwal (2410110354).

## Contents
| Path | Description |
|---|---|
| `FDS_Project.ipynb` | Complete pipeline (Sections 0-7); run top to bottom on Google Colab |
| `data/raw/` | Frozen raw snapshot: Google Trends (US, weekly), Yahoo Finance (daily), FRED (monthly), extraction log |
| `data/processed/` | Analysis-ready weekly and monthly panels |
| `tables/` | All result tables (CSV); `tables/paper/` holds the numbered IEEE tables (CSV + LaTeX) |
| `figures/` | All figures (PNG, 300 dpi) |
| `requirements.txt` | Package versions used |

## Reproducing the results
1. Open `FDS_Project.ipynb` in Google Colab and make sure the `data/raw/` folder is in `MyDrive/FDS_Project/`.
2. Run all cells. With the raw snapshot present, no API calls are made (`FORCE_REFRESH = False`), so the results are reproduced exactly. A FRED API key is only needed when re-downloading (`FORCE_REFRESH = True`).
3. Runtime: about 8 minutes on a standard Colab CPU (mostly Prophet walk-forward refits).

## Data sources
Google Trends (via pytrends), Yahoo Finance (via yfinance), and FRED, Federal Reserve Bank of St. Louis (series RSHPCSN, MRTSSM4482USN, RSCCASN). Study period 2020-01-01 to 2024-12-31. Random seed 42.
