# Analysis on Ecological Footprint

## Project motivation
Global Footprint Network, founded in 2003, is an independent think tank originally based in the United States, Belgium and Switzerland. It was established as a charitable not-for-profit organization in each of those three countries.

Global Footprint Network develops and promotes tools for advancing sustainability, including the ecological footprint and biocapacity, which measure the amount of resources we use and how much we have. These tools aim at bringing ecological limits to the center of decision-making.

This provides a great opportunity to understand the development of human consumption and biocapacity over time and 
The analysis of such dataset can reveal how the different levers of ecological footprint have developed and what ecological debtors and creditors are.

Hence, the purpose of this notebook is to do an EDA of the data provided from NFA and merge it with economical and energy-related data from the World Bank.

## Dataset
The dataset contained following files:
* `NFA_2018.csv` contains yearly data per country on ecological footprint and biocapacity broken down to their respective levers. Data has been sourced from [Kaggle](https://www.kaggle.com/footprintnetwork/national-footprint-accounts-2018)
* `world_bank.csv` contains various country data over time on CO2 emissions, energy production and GDP. Sourced from [World Bank](https://data.worldbank.org/)

### Description of files
- `analysis.ipynb` contains the steps performed during the analysis
- `analysis.html` is an HTML rendering of Jupyter notebook analysis.ipynb


### Libraries used in the project
- `pandas` to store and process dataframes created from datasets
- `numpy` to perform some operations on underlying multidimensional array backing the dataframe in Pandas
- `matplotlib` to create plots for showing graphical visualizations of analysis
- `seaborn` to create special types of data visualizations like Heatmap
- `geopandas` to create interactive maps
- `requests`, `json` and `zipfile` to download necessary geo data

I followed the steps recommended in [CRISP-DM](https://en.wikipedia.org/wiki/Cross-industry_standard_process_for_data_mining) methodology to explore this dataset, perform necessary transformations, extracting features and prepare data.


## Analysis

The full analysis can be found in `analysis.html`

The following question were tried to be answered:

1. What is the relationship of biocapacity and ecological footprint over time?
2. How have footprint and biocacapcity as well as ecological debtors and creditors developed over time?
3. How did CO2 emissios per sector develop?
4. what is the relationship of CO2 per Capita and GDP per Capita?

## Conclusion

1. Since the 1970's our ecolocical footprint (Demand) is higher than Earth's biocapacity (Supply)
2. This is being reflected in the number of ecological debtors and creditors. In 1960 there were 70% creditors, a relationship which reversed to 70% debtos
3. Carbon emissions are the major driver of this development.
4. The amount of CO2 for Electricty and heat production has increased over the six-fold over the last 40 years stressing the importance of decarbonizing our electricity production.
5. This part reflects also the strong correlation of 0.8 between CO2 emissions per capita and GDP per capita.

## Acknowledgement

A big thank you to the Global Footprint Network for providing a ton of resources and great data!
