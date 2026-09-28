# Python Data Science & ML Projects

A cleaned portfolio archive of Python notebooks and research prototypes covering data science, machine learning, NLP, web/API data collection, epidemiology, and medical imaging.

## Repository map

| Folder | Focus |
|---|---|
| `notebooks/foundations/` | Small data-science exercises, including wine-quality exploration |
| `notebooks/machine-learning/` | Regression, decision trees, Naive Bayes, MNIST neural networks, and IMDB LSTM experiments |
| `projects/financial-news-sentiment/` | NYT headline collection + stock-price/sentiment exploration |
| `projects/steam-review-analysis/` | Steam/EA scraping, review collection, and exploratory analysis |
| `projects/sars-cov2-analysis/` | Epidemiology/genomics experiments, survival analysis, and selected generated results |
| `projects/mednist-classification/` | MONAI/PyTorch medical-image classification experiment |

## Public-repository cleanup

The original folder was a long-running personal workspace rather than a GitHub repository. Before packaging it, I:

- removed nested `.git` histories and notebook checkpoints;
- cleared notebook outputs and execution state;
- removed a hard-coded NYT API key and replaced it with `NYT_API_KEY`;
- replaced local `/Users/...` paths with relative project paths;
- excluded the MedNIST dataset and other large third-party/raw datasets;
- excluded large generated SARS-CoV-2 CSVs and mixed-source viral metadata;
- excluded scraped/retrieved NYT, stock, and Steam CSVs from redistribution;
- excluded an old Django personal website containing personal photos, documents, and a SQLite database;
- excluded two copied DPhi NumPy bootcamp notebooks because they were primarily third-party instructional material rather than original portfolio work.

## Environment

A broad dependency list is provided in `requirements.txt`. Individual notebooks use only subsets of these packages.

```bash
python -m venv .venv
source .venv/bin/activate      # Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

Jupyter can then be launched with your preferred notebook environment.

## Reproducibility

This repository is an archive of projects created across different periods, so not every notebook is guaranteed to reproduce exactly against current APIs or package versions. Each substantial project includes a short README describing omitted datasets or setup requirements.

## Security

No API credentials should be committed. The NYT project reads the key from the `NYT_API_KEY` environment variable; use the included `.env.example` only as a template.
