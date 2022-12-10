# project-01

The data source for this project is from the US Energy Information Administration (EIA). The EIA is a part of the US Department of Energy and is dedicated to the collection and sythnthesis of information regarding the production, usage, and cost of energy within the United States. The EIA has an API found at https://www.eia.gov/opendata/browser/electricity/state-electricity-profiles that we used to collect our datapoints. We used this data source to answer some key questions regarding energy production between the years of 2008 and 2018:
1. How have energy costs changed over the course of the time period by state?
2. How have CO2 emissions per megawatt hour changed over the time period by state?

We elected to primarily examine CO2 emission per mw hour rather than net CO2 emission, as we believed that examining net emissions could obfuscate a state's efforts to decrease CO2 emissions over the time period. For example Texas in 2018 was the number 1 net carbon emitter in the United States. However when examining the state's CO2 emission per mw hour against the average across the country Texas falls close to the mean of 998.76 lbs of of CO2 emitted per MW hour produced at 1060. This difference could be explained by Texas being more populous or industrious, requiring a larger net consumption of energy, and therefore producing a larger net amount of CO2.

To analyze those questions we looked at the average price and CO2 emission datapoints for each state at the beginning and end of the time period. We extracted:
  1. The top and bottom 5 states in each metric
  2. The state that most closely matched the mean and median of each metric
#  3. The percent change in each datapoint in each state over the time period

