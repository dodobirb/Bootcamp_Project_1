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

To review the analysis files simply clone the repository and run the files in the following order after launching Jupyter Lab or VS Code from any CLI (Git BASH, Conda, Miniconda, Powershell, etc.) to step through the data analysis **yahoo_data_download_csv_analysis_plot_1.ipynb, stocks_to_mort_analysis_plot_2.ipynb, and Mortgage delinquency rates analysis.ipynb** with:

Upon launching the Jupyter notebook files you will step through the analysis one code block at a time. 

---

## Contributors

In this section, list all the people who contribute to this project. You might want recruiters or potential collaborators to reach you, so include your contact email and, optionally, your LinkedIn or Twitter profile.

---

## License

When you share a project on a repository, especially a public one, it's important to choose the right license to specify what others can and can't with your source code and files. Use this section to include the license you want to use.




"""SEE MODULE 2 CHALLENGE README.md IN GITHUB FOR THIS TEMPLATE IN USE"""
