# Link between Simpsons sentiment and sentiment in mass media in USA(1990-2017)


## Data Gathering

1. `NYT_articles_links.ipynb` - gathering links for articles from 1990 to 1999 using New York Times API, 1000 articles for each year 
2.  `NYT_articles.ipynb` -  for each link gathered at step above, we parse an article, so after step 2 we have dataset in format date:text


## Preprocessing

1. `Articles_preprocessing.ipynb` -  preprocessing of 1990-1999 data
2.  `Group_by_year_and_month.ipynb` -  from raw articles we find average sentiment score for each given month, but because we have a huge dataset, it's splitted into 21 time series chunks
3.  `Merge_chunks_into_one_time_series.ipynb` - merge 21 time series chunks into one time series, plus some missing values imputation

4. `Preprocess_and_make_time_series_from_scripts.ipynb` - get monthly  sentiment score for Simpsons scripts

## Analysis

1. `Analysis.ipynb` -  obtaining analiyic results of this research 