# The Reactions of the German Stock Market to COVID-19 and Containment Policies: A Vector Autoregressive Analysis

## Documents:

Notebooks:
*  **01-data-preparation.ipynb** *(fetching, joining and preparing the data for further analysis)*
*  **02-data-descriptive.ipynb** *(generating descriptive statistics and plots for the prepared and non-transformed data)*
*  **03-find-stationary-timeseries.ipynb** *(scripts to find suitible data transformations for stationarity of the variables to use in VAR Model)*
*  **04-var-models.ipynb** *(VAR model specification, estimation and diagnosis)*

.csv files:
* **hdax-data.csv** *(Source data on the German HDAX index from investing.com)*
* **owid-covid-data.csv** *(Source data on the Covid-19 pandemic from OurWorldInData)*
* **prepared_data.csv** *(joined and cleaned data)*
* **prepared_data_sample_1.csv** *(joined and cleaned data for the first infection wave)*
* **prepared_data_sample_2.csv** *(joined and cleaned data for the second infection wave)*
* **prepared_data_sample_full.csv** *(joined and cleaned data for the full sample time frame)*
* **transformed_data_sample_1.csv** *(data ready for input into VAR-Model for the first infection wave)*
* **transformed_data_sample_2.csv** *(data ready for input into VAR-Model for the second infection wave)*
* **transformed_data_sample_full.csv** *(data ready for input into VAR-Model for the full sample timeframe)*

Plots:
* *(all plots are exported from above mentioned notebooks)*

pdf_code:
* this folder includes all notebooks exported as pdf files *

## Introduction:

The infectious respiratory disease Covid-19 caused by the novel coronavirus SARS- CoV-2 has been taking its toll on the health of people and economies worldwide. Since its emergence in late 2019 in the Chinese city of Wuhan (Sohrabi et al., 2020), the virus rapidly spread across borders leading to a contraction among millions of people. Governments around the world swiftly reacted by instituting unprecedented containment measures. By March 2020, more than 100 countries have introduced massive non-pharmaceutical interventions (NPIs) including full or partial lockdowns (Hale et al., 2021), social distancing measures, as well as local, national, and international moving restrictions.

While the world has certainly seen various different pandemics over the last century, Covid-19 remains largely unprecedented in its effects on the economy and financial markets (Baker et al., 2020). On the one hand, this is because pandemics can cause immense uncertainty and disruptions to business (Correia, Luck, & Verner, 2020), while on the other hand, government instituted containment measures massively influence the economic trajectory of societies.

For Germany, having an economy that is highly dependent on export and international supply chains, a global pandemic like this can have detrimental consequences. As an emergency reaction, German federal and state governments mandated closures of schools, universities, and businesses and put in place a wide array of containment and health measures such as mandatory social distancing rules, testing campaigns, and quarantine policies. At the same time, the country’s government has been rolling out support and stimulus packages, including tax cuts, to support the national economy. In fact, the German fiscal response to the economic fallout has been among the largest worldwide (IMF Fiscal Affairs Department, 2021).

Due to the far-reaching consequences of Covid-19 and the inherently conflicting goals that emerge when trying to contain the virus, the pandemic has drawn a lot of attention to the relationship between economics and public health decisions. While the long-term consequences of the pandemic are still hard to predict, financial markets offer a unique and timely perspective on the state of the economy. Due to the stock market’s ability to provide useful information in fast-evolving and complex situations (Wagner, 2020), its reaction to changes in the trajectory of the pandemic can be an important indicator to different stakeholders, including political decision-makers.

Because of the complex emergency situation and a large variety of different government instituted measures, it is, however, not obvious how and why financial markets reacted to the pandemic. While during February and March 2020, global stock prices dropped and experienced extreme volatility with a magnitude comparable to the great financial crisis of 2008 and the black Monday of 1987 (Baker et al., 2020), they quickly rebounded and even reached new all-time highs in the months thereafter.

To better understand how the Covid-19 pandemic influenced the German financial market, this study sets out to analyze the stock market’s reactions to the trajectory of the pandemic and related containment and health measures. Specifically, this study tries to extract information from forward-looking asset prices by fitting a vector autoregressive model to stock price data, a policy stringency index, and daily news on reported Covid-19 cases. The significance, timeliness, and direction of the reactions and changes in reactions over time are of primary interest.

The remainder of this study is organized as follows: First, related literature is examined to arrive at a working hypothesis. Thereafter, already existing empirical literature in the context of Covid-19 will be considered in light of the previously established hypotheses. As the last step, a vector autoregressive model is estimated and interpreted with Granger causality tests and impulse response functions. A critical review and outlook on the results is given in the end.


