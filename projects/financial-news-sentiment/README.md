# Financial News Sentiment Exploration

Exploratory notebooks connecting historical stock-price data with New York Times headline sentiment.

## Included work

- NYT Article Search API collection
- stock-price collection with `yfinance`
- headline cleaning/combination
- VADER/TextBlob-style sentiment exploration
- topic/sentiment experiments

## API key

The original notebook contained an API key directly in a code cell. It has been removed. Set your own key before running the collection notebook:

```bash
export NYT_API_KEY="..."
```

## Data

Historical headline and stock CSVs from the original working folder are not redistributed here. Recreate them with the included collection notebooks and respect the current terms of the upstream data providers.
