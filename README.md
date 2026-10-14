# Industry Oriented Projects

Industry Oriented Projects is a collection of Python notebooks for exploring demand forecasting, social-media engagement, and historical stock data.

## Notebooks

| Notebook | What it contains | Data or service |
| --- | --- | --- |
| `Demand Forecasting /Demand forecasting using py.ipynb` | Demand/inventory plots, SARIMAX forecasting, and example reorder calculations | Included `Demand Forecasting /demand_inventory.csv`; upload through Colab |
| `In_depth_Twitter_Retweet_Analysis.ipynb` | Retweet distributions, hourly/weekday summaries, correlations, and plots | Included `In-Depth Twitter Retweet Analysis Dataset.csv` |
| `Algorithmic Trading bot/Algorithmic trading bot.ipynb` | Historical AAPL data retrieval, classification models, and draft strategy-return calculations | Polygon market-data API account and API access |

## Getting started

The notebooks use pandas, NumPy, Matplotlib, seaborn, Plotly, statsmodels, and scikit-learn. The trading notebook additionally installs `polygon-api-client`. No shared dependency manifest or pinned environment is provided.

Use Google Colab for the upload-based demand notebook, or open the collection in an existing Jupyter environment:

```bash
jupyter notebook
```

- For demand forecasting, upload the included CSV when prompted.
- For retweet analysis, upload the included CSV to `/content/` in Colab or change the first cell's path for local use.
- For the trading notebook, use your own Polygon credentials and check your account's historical-data access. Service charges or plan limits may apply.

Run cells in order and inspect each notebook's assumptions before interpreting its plots.

## Status and limitations

These are learning notebooks, not deployed applications. The trading notebook does not place trades. It contains an inline credential that should be removed and rotated before further use or sharing, an undefined `decision_tree` reference, and later calculations that assume earlier cells succeeded. Its random data split and example return calculations are not evidence of a viable trading strategy.

Demand inventory settings and retweet timestamp construction use example assumptions. Dataset provenance and reuse licenses are not documented. There is no automated test suite.

## License

No license file is included.
