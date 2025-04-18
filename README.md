# Data Matcher App

A Streamlit application for comparing and matching records between two datasets using fuzzy matching algorithms.

## Features

- **Upload Multiple Formats**: Support for CSV and Excel files (XLS, XLSX)
- **Visual Field Mapping**: Visually connect related fields between datasets
- **Flexible Matching**: Multiple similarity algorithms and configurable threshold
- **Customizable Output**: Select which fields to include in the results
- **Interactive Results**: View and filter matching results
- **Excel Export**: Download results as a formatted Excel file

## How It Works

1. **Upload Data**: Upload two datasets (CSV or Excel files)
2. **Map Fields**: Create connections between related fields in both datasets
3. **Configure Matching**: Set the similarity threshold and matching method
4. **Select Output Fields**: Choose which fields to include in the final results
5. **Process Data**: Run the matching algorithm
6. **Review & Export**: Examine results and download as Excel

## Matching Methods

- **Jaro-Winkler** (Default): Good for names and short text with typos
- **Levenshtein**: Good for comparing strings with insertions/deletions
- **Partial Ratio**: Good for finding substrings
- **Token Set Ratio**: Good for text that may be in different orders

## Use Cases

- Customer database deduplication
- Address verification
- Product catalog matching
- Employee record reconciliation
- Contact list consolidation

## Deployment

### Running Locally

1. Clone this repository
2. Install dependencies: `pip install -r requirements.txt`
3. Run the app: `streamlit run app.py`

### Deploying to Streamlit Cloud

1. Fork this repository to your GitHub account
2. Log in to [Streamlit Cloud](https://streamlit.io/cloud)
3. Create a new app and select your forked repository
4. Deploy the app

## Requirements

- Python 3.8+
- Streamlit
- Pandas
- Numpy
- Rapidfuzz
- Openpyxl
- Plotly

## License

MIT