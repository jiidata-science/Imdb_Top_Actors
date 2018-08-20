# Exploring imdb’s most featured actors


## Introduction & Purpose

In this project we take a look at [IMDb's Top 250 rated movies](https://www.imdb.com/chart/top). More specifically, in this article, we scrape IMDb's top rated movies, along with their corresponding cast & crew listings, and explore who the "real movie superstars" are - essentially, *which actors feature in the most/multiple top rated movies?* 

I began this project with the naive assumption that these "superstars" would all be well-known household names; the likes of *Katharine Hepburn, Robert De Niro* and *Jack Nicholson* - similar to IMDb's list of [100 greatest actors & actresses of all time](https://www.imdb.com/list/ls053085147/) - **BUT this analysis resulted in some suprising finds!**

For this project we used Python, and a selection of libraries, for data collection, exploration and visualisation. This article includes a selection of Python code-blocks and visualisations that help us to explore and draw insights from the data. The full codeset is available on [Github](https://github.com/jiidata-science/Imdb_Top_Actors) as a Jupyter notebook.

### Motivation

So why did I chose to explore this random and niche topic? Well, primarily I wanted to demonstrate use of web scraping technology to collect data that wasn't otherwise readily available in the desired format (yawn!). The second reason was merely because I enjoy watching movies - *hardly a unique interest* - so, I was inately interested in the data itself.

### What we'll be looking at

  * Part 1 (of 5): Importing Required Python Libraries
  * Part 2 (of 5): Data collection - Scraping IMDb's Top 250 Rated Movies, [using BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
  * Part 3 (of 5): Data collection - Scraping Movie Genre & Full Cast + Crew, [using BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
  * Part 4 (of 5): Data Exploration - Visualising Movie Ratings, with [Pandas](https://pandas.pydata.org/) and [Plotly](https://plot.ly/python/)
  * Part 5 (of 5): Data Exploration - *Who Really Are The Best Actors?*, with [Pandas](https://pandas.pydata.org/) and [Plotly](https://plot.ly/python/)

### Codeset

The full codeset is available in the [Imdb_Scraping_Analysis jupyter notebook](https://github.com/jiidata-science/Imdb_Top_Actors/tree/master/Code). This is (intentionally) well commented to ensure ease of reproducibility.

### Pre-requisites

#### Python version
Python version 3.6.3, with Anaconda distribution

#### Required Python Libraries
A step by step series of examples that tell you how to get a development env running

``` shell
# libraries for requesting and scraping web pages
certifi==2018.4.16
urllib3==1.22
beautifulsoup4==4.6.0

# libraries for structuring data
pandas==0.22.0
numpy==1.12.1

# libraries for fitting models/relationships (exploratory analysis)
scipy==1.0.0
plotly==3.1.0
```