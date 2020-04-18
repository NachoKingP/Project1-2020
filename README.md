# Project 1 - Compare U.S Financial Market Most Recent Recessions
Dec. 2008 through Feb. 2009— (Housing Bubble) vs. Jan. 2020 through Mar. 2020- (COVID-19)

# Group Members
    Zahra Ahmadi, Sumeet Maheshwari, Brian Remite, and Bryan Wilson

# Prerequisites for running code
    The following modules must be installed to plot all our graphs
        plotly - pip install plotly
        chart_studio - pip install chart_studio
        yfinance - pip install yfinance

# File Structure
    Folders
        data_files - Stores all data sources we used to pull code and generate plots
            internet_sources - Stores all files that we gathered from internet sources
            output - All files we generated from within our code, to be used in other code
        documentation - Folder containing files we used to organize the project, including a project outline, as well as a folder with a
                tasklist.
        final_code - Folder containing our final jupyter notebooks, which I will detail below
            linregress.ipynb - Generates the linear regression chart that compared COVID-19 cases to DJIA index
            States_Unemployment_Rate.ipynb - Generates US heatmap for Unemployment rates.
            stock_charts.ipynb - Generates individual stock data charts for 2008 and 2020 recessions
            stockdataload.ipynb - loads in djia stock data and generates graphs
            Stock market.ipynb - Generates plots for the stock market data
            UE_barcharts.ipynb - Generates barcharts for the Unemployment data created in unemployment-development.ipynb
            unemployment-development.ipynb - loads data from trendingeconomics.com and parses data, generating two files for other code
                charts.  Also pulls in COVID data and parses that, generating two charts.
            Unemployment_Rate-map.html - Heatmap of US showing unemployment rate data per state.
        Old Presentations - This folder contains our drafts of the presentation.
        output - Folder containing all charts in image form, ready for viewing.

# Hypothesis
The 2020 recession has been worse statistically, both in terms of the percentage of value lost in the stock market, as well as the unemployment rate (in both total number of unemployed persons, as well as the percentage of U.S. population facing unemployment.)

# Method
We will utilize publicly available data on the internet to collect information on the DJIA in both 2008 and 2020, the unemployment rates in 2008 and 2020, and data on how the COVID cases developed over time. We will compare the two timeframes using this data, plot out graphs to visualize what we have found, and come to a conclusion.
    
# Conclusion
The linear regression plot of the DJIA vs. COVID cases showed that there was a P-value of .002, meaning that there is less than a 1% chance of the variation being random, however the R-squared value was .20, meaning that there was approximately 20% of the variation around the mean within the data.  This shows us that there is a correlation, but not a linear correlation between those two data sets.

Our data on unemployment is incomplete, as the unemployment rate for April is as-of-yet unavailable. The data through March showed a trend towards correlation, however there is preliminary April data that shows the number of unemployed will skyrocket by the end of this month.

Based on the time period we have available to us for COVID-19, with only 3 months of complete data, there is a trend towards showing that our hypothesis was in fact correct.  However, at this time, we can not make a definitive conclusion due to the fact that the 2020 recession is ongoing, and we would need the data for the whole recession to do so.

# Sources
DJIA Data: Yahoo Finance https://finance.yahoo.com/quote/%5EDJI/history?

Stock Data: Yahoo Finance API pip install yfinance

COVID Data: The New York Times https://github.com/nytimes/covid-19-data

Unemployment Data: tradingeconomics.com https://tradingeconomics.com/united-states/unemployment-rate

Unemployment Rate by State: https://www.bls.gov/

Data Plot Sources: https://plotly.com/, https://pypi.org/project/chart-studio/
