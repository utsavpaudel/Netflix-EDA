# Netflix Data

This directory contains the Netflix datasets used for exploratory data analysis.

## Files

### netflix_data.csv
Complete Netflix catalog data including:
- **show_id**: Unique identifier
- **type**: Movie or TV Show
- **title**: Title of the content
- **director**: Director name
- **cast**: Cast members
- **country**: Country of origin
- **date_added**: Date added to Netflix
- **release_year**: Year of release
- **duration**: Duration in minutes (movies) or seasons (TV shows)
- **genre**: Content genre/category
- **description**: Content description

### color_data.csv
Auxiliary data file for color mapping in visualizations.

## Data Source

The Netflix data is publicly available and commonly used for educational purposes in data analysis courses and projects.

## Usage

```python
import pandas as pd

# Load Netflix data
df = pd.read_csv('data/netflix_data.csv')
print(df.head())
```
