# wikipedia-scraping-companies
Scraping and analysing Wikipedia tables of the largest companies by revenue (BeautifulSoup + pandas), with a reusable scraper and an African industry analysis.


## What this project does
- Scrapes Wikipedia tables of the largest companies by revenue using
  BeautifulSoup and pandas.
- Uses one function, `scrape_wiki_table(url, must_have)`, which picks the table
  by its column names instead of its position on the page.
- Cleans the data (text to numbers) and analyses revenue by industry for
  African companies.

## Main findings
- Oil and gas is the largest industry (119.3 bn USD), with Sonatrach
  alone contributing about 65%.
- Some companies in the list are subsidiaries of others in the same list,
  so I compared totals with and without them. Oil and gas stays first either way;
  second place changes.

## Files
- `Scraping_Data_from_Wiki.ipynb`: the full code and written analysis
- `africa_companies_by_revenue.csv`: the cleaned data
- `africa_industry_comparison.png`: chart comparing totals with and without subsidiaries

## Limitations
- The Wikipedia source has some inconsistent rows (for example Ethiopian
  Airlines' rank and revenue do not match).
- My list of subsidiaries is a judgment call and may be incomplete.

## How to run
Open the notebook in Jupyter and use Kernel → Restart & Run All.
Requires: requests, beautifulsoup4, pandas, matplotlib.
