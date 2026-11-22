# Final summary of results

## H1: lead-lag (prewhitened CCF, Haugh test, BH-FDR q < 0.05)
- Stocks, brand -> own stock (Family A): 0 of 6 pairs significant. **Not supported.**
- Stocks, within-niche (Family B): 0 of 52 pairs with a significant search lead. **Not supported.**
- Retail sales (Family C): 4 of 12 pairs significant in the primary test; robust to COVID/base-effect checks: rare beauty → RSHPCSN, hoka → MRTSSM4482USN; robust after seasonal adjustment of search: none.

## H2: Granger causality (search -> market, BH-FDR q < 0.05)
- Stocks (Family B): 0 of 52 pairs. **Not supported.**
- Reverse direction (market -> search) in Family B: 4 of 52 pairs (Granger or CCF).
- Retail sales (Family C): 2 of 12 pairs in the primary test.

## Forecasting (out-of-sample 2024, walk-forward)
- Stocks: naive random walk is the most accurate model for 9 of 13 stocks. Adding search changes RMSE by +0.9% (ARX vs AR) and +4.3% (Prophet), with 0 statistically significant improvements.
- Retail sales: best model per series: RSHPCSN: ARX YoY (search) (3.23% MAPE); MRTSSM4482USN: AR(1) YoY (6.53% MAPE); RSCCASN: Seasonal naive (2.20% MAPE).
- Seasonally adjusted search: ARX vs AR mean ΔRMSE +168.6% (original +104.0%); Prophet mean ΔRMSE +0.0%.

## Cross-sector growth
- Viral Skincare & Beauty: search +46%/yr; Functional Beverages: search +62%/yr; Comfort & Performance Footwear: search +23%/yr; Resale vs. Fast Fashion: search +11%/yr.