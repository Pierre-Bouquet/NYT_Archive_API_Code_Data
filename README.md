# NYT Archive API - Code & Data

Data from: [https://developer.nytimes.com/](https://developer.nytimes.com/docs/archive-product/1/overview)
The API is limited to 500 requests a day, here's all the data you'll need <3

Includes: 
- Code in python to fetch the data from the Archive API of the NYT Times
- Raw NYT archive data ; 1851 - 2023
- Cleaned archive data ; 1851 - 2023 

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
{'headline', 'abstract', 'pub_date', 'web_url', 'keyword_1', 'keyword_2', 'keyword_3', 'keyword_4', 'keyword_5'}



