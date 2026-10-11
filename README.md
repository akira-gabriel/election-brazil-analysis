# Election Brazil Analysis
Exploring correlations and predicting votes in Brazilian elections

## Research Questions
1 - Is it possible correlate social government projects to numbers in candidates?
2 - Wich factors are strong and weak correlated?

## Data
- Source: TSE Open Data Portal (https://cdn.tse.jus.br/)
- Files used: Presidential votes by polling sections by years (election years to be defined)

## Tech Stack
| Layer | Tools | Why |
|---|---|---|
| Language | Python 3.11 | One of the best languages for data analysis, with a rich ecosystem |
| Data | pandas, numpy | Solid choices for data cleaning and transformation |
| Modeling | scikit-learn | Pipelines, cross-validation and metrics |
| Visualization | plotly, seaborn | Fast exploratory and interactive charts |
| App / Deploy | Streamlit | Turns the analysis into a shareable demo |
| Versioning | Git, GitHub | Reproducible history and collaboration |

## Project Structure
data/raw/   -> original TSE files
notebooks/  -> exploration and collection
src/        -> reusable code
tests/      -> unit tests

## How to run
1. git clone https://github.com/akira-gabriel/election-brazil-analysis.git
2. uv venv && uv pip install -r requirements.txt
3. Run notebooks/collect.ipynb to download the data

## Timeline
| # | Milestone | Time | Deliverable |
|---|-----------|------|-------------|
| 1 | Data collection and cleaning | 2-3 days | Download files, clean, select relevant columns, standardize, aggregate and save as parquet. |
| 2 | Exploration and statistics | 3-4 days | Distributions, hypothesis tests, correlations, merging with IBGE data. |
| 3 | Visualization | 2-3 days | Using relevant charts, like histograms, scatterplots, etc. |
| 4 | Machine learning | 4-5 days | Prepare data, test some models, temporal validation, interpretation. |
| 5 | Deploy and documentation | 2-3 days | Build a simple Streamlit app, final analysis, results, limitations and possible next steps |

## Status
- [x] Project plan
- [ ] 1. Data collection and cleaning
- [ ] 2. Exploration and statistics
- [ ] 3. Visualization
- [ ] 4. Machine learning
- [ ] 5. Deploy and documentation