---
title: Report on Analysis
sidebar: mydoc_sidebar
permalink: apmc_analysis.html
folder: mydoc
---

## Objective

To understand the effect of MSP on market prices of different commodities at Mandi level and aggregate state level. To analyse the variation in Mandis across the state in terms of implementation of MSP and Procurement scheme. We first break down our objectives into specific questions to answer from the data available.

* Which APMC Mandis are experiencing more negative deviations from MSP taking into account all MSP linked agriculture produce over three years?
* Which APMC and for what commodity there is large price fluctuation in a given season and year ?
* How are prices of different commodities varying across Mandis in over time ?

## Methodology

  We start with some data sniffing to remove outliers and NAs. Then we saw price fluctuations of every commodity averaged across Mandis to get an idea of [trend and seasonality component]({{site.baseurl}}/pages/vis/avg_across_mandis_for_each_commdty.html) in the time series. We observed that there is almost constant trend in commodity prices. So simple averaging was used to estimate trend component. Also every time series of APMC-commodity combination was tested for additive and multiplicative seasonality and flagged accordingly. [Residuals]({{site.baseurl}}/pages/vis/avg_resi_across_mandis_for_each_commdty.html) in each case were estimated. 

After preliminary data cleaning, we try to answer questions mentioned above in that order as given below: 

* [MSP deviation CDF]({{site.baseurl}}/pages/vis/cdf-dataset.html): Firstly, we calculate the relative deviation of market price from MSP for every APMC taking all commodities coming under MSP over the span of three years. Then a simple CDF of these observations gives a good understanding of deviation of market prices from MSP. 

* Price fluctuations: We measure fluctuations by range (difference of  max and min) of prices for a particular commodity in a given Mandi. For this we average price ranges over relavant period - season or year.
   
* [Price Variation]({{site.baseurl}}/pages/vis/stddev_across_mandis_for_each_commdty.html): We use standard deviation of prices across mandis in a given month to measure variation. Then we plot this variation over time for all commodities.
`

## Results

* We observe that there is no substantial trend in market prices over years. This might be reason for unrest among farmers in recent years. They are distressed with stagnation of income coupled with increase in input costs and inflation.
* Another important observation is negative deviation from MSP. We see that for most of the commodities market price has been consistently below MSP in majority of Mandis. This indicates how MSP is not acting as a floor as intended.
* We find significant price variation across Mandis for many commodities like chillies, turmeric. This indicates how low density of Mandis along with poor connectivity can influence prices for the same commodity in the same state.   



{% include links.html %}
