# Baobab Ethical Fund Modelling

The project in this repo was undertaken to assist [Inves](https://www.inv.es/), a new-breed financial services company, determine if their ethical fund was financially viable as an investment vehicle.

Passive investment funds are a popular financial instrument, however the companies that are included in these schemes are often the subject of controversy (e.g. Steinhoff), engage in dubious business practices or create products that have a nett harmful effect on the world or those that use them (e.g. British American Tabacco). The Babab eithical fund aims to provides a low-cost investment scheme that allows investors to avoid funding companies deemed harmful or unethical. Essentially, the fund consists of the companies listed on the JSE, with unsuitable companies excluded. This model aims to determine if the Baobab ethical fund would outperform the Johannesburg Stock Exchange (or a pared-down version of it) over a period of 5 financial years.

A list of JSE-listed companies is imported. Some companies are removed due to missing historical data. The Baobab ethical fund is compared to these companies, as well as the JSE as a whole to confirm that the missing company data doesn't affect the prediction. When making the comparisons between the pseudo-JSE and the Baobab fund, each is modeled as an equal-weighted fund in the absense of information about numbers of shares available for each company. The actual JSE all-share price, however, takes the number into account. As such, the pseudo-JSE (calculated as an equal fund) and actual JSE all-share price are shown on each chart for comparison.

Baobab is constructed by starting with the pseudo-JSE model (350 companies) and removing a further 60 companies that are deemed to not meet the ethical criteria for inclusion.

At each day, the price of each (the JSE and Baobab) are obtained by summing the value of stocks registered with each. Then two simulated buying scenarios are created:
* Dollar-cost averaging: 30x R10,000.00 = R300k investment
* Single-shot R300k innvestment on Day 1

The performance of these is analyzed over an approximate 5 year period, starting in 2013, and plotted against one another.

The following image shows the charts for the dollar-cost averaging investment schedule, indicating comparative performances for the five-year period. It indicates that the fund would, in fact, have out-performed the JSE over the last five years.

![Comparison plot](https://raw.githubusercontent.com/MProx/Baobab_Ethical_Fund/master/ComparisonPlot.png)


### Usage instructions:
The model is presented in .ipynb format, to be opened using Jupyter Notebook.
The following libraries are required to run the Python 3.5 code:
* Pandas
* Numpy
* Matplotlib
* Plotly

Once opened in Jupyter Notebook, display all charts by clicking Kernel > Restart and Run All
