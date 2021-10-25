# Bootcamp_Project_01

banks chosen:
https://www.ffiec.gov/npw/Institution/TopHoldings

metro area mortgage delinquency rates, 2008 - march 2021:
https://www.consumerfinance.gov/data-research/mortgage-performance-trends/download-the-data/

using yfinance:
web scraper: acess data in a more pythonic way
https://pypi.org/project/yfinance/
*Reagrding the monthly date of bank stocks' prices: due to the limitations of yfinance's "interval" parameter, the first date of each subsequent month is used in place of the last date of the month in question in the data.*

*Example: 2010-02-01 stock prices are analysed in correlation to 2010-01-01 - 2010-01-31 (monthly) mortgage delinquency rates.*

using cartographic boundary files from the US census bureau:
https://www.census.gov/geographies/mapping-files/time-series/geo/cartographic-boundary.html


TEMPLATE:

# Project Title

Just after the title, introduce your project by describing attractively what the project is about and what is the main problem that inspires you to create this project or what is the main contribution for the potential user of your project.

---

## Technologies

Describe the technologies required to use your project such as programming languages, libraries, frameworks, and operating systems. Be sure to include the specific versions of any critical dependencies that you have used in the stable version of your project.

This project leverages python 3.8.8 with the following packages:

* [geopandas](https://geopandas.org/getting_started/install.html) - For creating dataframes and conducting data analysis from a varity of geospatial data formats. Follow link for more information about this library.

* [hvplot](https://hvplot.holoviz.org/) - For interactive visualizations. Follow link for more information about this library.

* [geoviews](https://geoviews.org/) - For geocentric interactive visualizations. Follow link for more information about this library.

* [holoviews](https://holoviews.org/) - For annotated and interactive visualizations. Follow link for more information about this library.

* [cartopy](https://scitools.org.uk/cartopy/docs/latest/) - For cartographic overlays used in geospatial visualizations. Follow link for more information about this library.

* [pandas](https://pandas.pydata.org/) - For creating dataframes and conducting data analysis from a varity of data sources. Follow link for more information about this library.

* [pathlib](https://docs.python.org/3.8/library/pathlib.html) - For navigating file system paths. Follow link for more information about this library.

* [yfinance](https://github.com/ranaroussi/yfinance) - For downloading stock data. Follow link for more information about this library.

---

## Installation Guide

In this section, you should include detailed installation notes containing code blocks and screenshots.

```python
  pip install geopandas
  pip install pandas
  pin install hvplot
  pip install cartopy
  pip install geoviews
  pip install holoviews
  pip install yfinance 

  The other libraries should be part of the standard Python installation. 
```

---

## Usage

This section should include screenshots, code blocks, or animations explaining how to use your project.

To review the analysis files simply clone the repository and run the files in the following order after launching Jupyter Lab or VS Code from any CLI (Git BASH, Conda, Miniconda, Powershell, etc.). Upon launching the Jupyter notebook files you will step through one code block at a time. 

First run **yahoo_data_download_csv_analysis_plot_1.ipynb**




Next run **stocks_to_mort_analysis_plot_2.ipynb** 





Finally run **Mortgage delinquency rates analysis.ipynb**

There are 15 code blocks in total with a brief summary of each section.

* #1: Imports all relevant libraries for data wrangling, data visualizations, and data analysis
* #2: Imports, cleans, and formats "Mortgage performance trends" data from https://www.consumerfinance.gov/data-research/mortgage-performance-trends/download-the-data/
    Imports, cleans, and formats "CBSA codes and polygonal geometry coordinate" data from https://www.census.gov/geographies/mapping-files/time-series/geo/cartographic-boundary.html
    Displays combined dataframe on screen and exports to excel file. The dataframe is used in code blocks #3 to #6
* #3 to #6: Generates multiple cartographic map of 200+ metro areas average mortgage delinquency rates in 2008 and 2020 to present a visual representation of the data. Code block #6 presents two maps side-by-side to provide a visualization to view 2008 vs 2020.
* #7: Re-cast the dataset as a new dataframe to build time-series, scatter, and boxplot charts used in code blocks #8 to #11
* #8: Creates an interactive time series line plot and data table for mortgage delinquency rates by metro area  
* #9: Provides the range of average rates to visualize the range across all 200+ metro areas in a scatter plot
* #10: Provides the rolling 12-month average rates to visualize the trend across all time periods in a time series line plot
* #11: Generates multiple boxplots. First, one for every metro area (200+) using all data points. Second, interactive box plot to select an individual metro area and see a boxplot for each year from 2008 to 2021.
* #12: Import, clean, and format stock data to use for the correlation analysis from the yfiance python library. Also combine into a single dataframe for code blocks #13 to #15
* #13 to #15: Calculate scatter plots and correlation coefficients between the mortgage delinquency rate data and bank stock data. 
    *#13: All data used (2008 to March 2021) showing no correlation
    *#14: Portion of data used (2008 to 2010) showing a weak positive correlation
    *#15: Portion of data used (2018 to March 2021) showing a weak negative correlation.

---

## Contributors

In this section, list all the people who contribute to this project. You might want recruiters or potential collaborators to reach you, so include your contact email and, optionally, your LinkedIn or Twitter profile.

---

## License

When you share a project on a repository, especially a public one, it's important to choose the right license to specify what others can and can't with your source code and files. Use this section to include the license you want to use.




"""SEE MODULE 2 CHALLENGE README.md IN GITHUB FOR THIS TEMPLATE IN USE"""
