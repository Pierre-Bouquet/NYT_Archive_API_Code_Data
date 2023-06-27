# NYT Archive API - Code & Data

Includes: 
- Code in python to fetch the data from the Archive API of the NYT Times
- Raw NYT archive data ; 1851 - 2023
- Cleaned archive data ; 1851 - 2023 


## Data Source

Data from: [New York Times Developer](https://developer.nytimes.com/docs/archive-product/1/overview).

Please note that the data provided in this repository is sourced from the New York Times (NYT) and is subject to the terms and conditions set forth by the NYT. It is important to comply with the terms of use specified by the NYT. This data is intended for non-commercial use only, and the NYT retains full proprietary rights over it.

For more information about the terms of use, please refer to the [NYT Terms of Use](https://developer.nytimes.com/terms). The goal of this repository is to facilitate access to news data for the developer community.

## Code in Python

Jupyter notebook to be run at once.

Packages: 
- pandas                    2.0.2
- requests                  2.31.0 
- numpy                     1.24.3 
- tqdm                      4.65.0  

## Raw NYT Archive data

In monthly datasets to fit in GitHub file size limits.

## Cleaned NYT Archive data

In yearly dataset to fit in GitHub file size limits.

Removed columns: 
{"multimedia", "print_section","print_page", "source", "_id", "word_count", "uri", "snippet", "lead_paragraph"}

Kept types of articles:
{'Archives', 'An Analysis', 'Editorial', 'Interactive Feature', 'News', 'News Analysis', 'Newsletter', 'Op-Ed', 'Quote', 'Review', 'Slideshow', 'briefing'}

Kept: Top 5 keywords

Removed: "Motion pictures" from keywords

Output columns:
{'headline', 'abstract', 'pub_date', 'web_url',
"keyword_1", "keyword_2", "keyword_3", "keyword_4", "keyword_5", 
"keyword_6", "keyword_7", "keyword_8", "keyword_9", "keyword_10"}

## Notes

- The API returns an empty .json for months 8/1979 and 9/1979.



