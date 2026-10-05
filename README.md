# GDP Data Extraction and Processing

Extracts the top 10 largest economies by nominal GDP (IMF estimates)
and converts the values from million USD to billion USD.

## What it does
1. **Extract** – scrapes the GDP table from an archived Wikipedia page with `pandas.read_html`
2. **Transform** – keeps country and IMF GDP columns, selects the top 10,
   converts million → billion USD and rounds to 2 decimals
3. **Load** – saves the result to `Largest_economies.csv`

## Tools
Python, pandas, NumPy, Jupyter

## Files
| File | Description |
|---|---|
| `gdp_course_ver.ipynb` | Notebook with the full process |
| `Largest_economies.csv` | Output: top 10 economies (GDP in billion USD) |

## Notes
- Data source: Wikipedia snapshot from 2 Sep 2023 (via Wayback Machine),
  so the figures reflect IMF 2023 estimates.
- Based on the IBM *Python for Data Science, AI & Development* course project.

## Next step
An updated version using the IMF DataMapper API (2026 data) is in progress.
