**9/27/22**:
- Submitted abstract proposal
- Added resources to /etc/reference-list.md

To do:
- find EV electricity consumption data
- Continue finding literature on:
   -> Electricity consumption on California
   -> Approaches to electricity consumption prediction (regression...)
   -> EV electricity consumption
   -> California’s conventional car ban and its impacts

**10/5/22**:
- Created main.py file
- Added resources to /etc/reference-list.md
- Added EV data and CA driving distance data to /src folder
-    simple equation: CA_ec_t + CA_driven_t * proportion_ev_t * avg_ev_ec
-> CA_ec: current CA electricity consumption (predict over time)
-> CA_driven: total average miles driven in CA (predict over time?)
-> avg_ev_ec: average EV electricity consumption, 0.2 kWh/km
-> proportion_ev: proportion of cars that are EVs (predict over time)
- To calculate the amount of electricity consumed by EVs, do we take into account the exact models? i.e. 20% of sales are Tesla model Ys, 10% Nissan Leafs... which each have slightly different average kWh/km
-> taking the current average electricity consumption for EVs should be ok. Tesla sales are increasing, but overall, popular models have similar avg electricity consumption. If anything, as EV tech evolves, the average electricity consumption may go down, so using the current average will give us a slight overestimation.
-> after finishing this, try predicting major EV sales and taking them into account while calculating total EV energy consumption?
- Is just using proportion_ev accurate? Not all drivers drive the same distance, i.e. kind of general consumer (family vs. single, urban vs. rural...), truck drivers, other specialty drivers

To do:
- Complete main.py, generate predictions
- Look into distribution of types of drivers. Also, even after banning combustion engine sales, there will still be old gas cars around for a while

**10/15/22**:
- Searching for more robust dataset
- Added California weather dataset (2017-2020)
- Created account and API key for Energy Information Association's (EIA) API: https://www.eia.gov/opendata/browser/electricity
- Tried fetching "Supply and Disposition of Electricity" from "State Specific Data." Frequency: annual, data type: all (net generataion from commercial sectrion, net generation from independent power producers, combined heat and power...) in main.ipynb, but all data is coming back empty?

**10/16/22**
- Added readings (see 2018 disaggregation paper)
- All data from last week's site seemed to be empty, so looked into new sources; downloaded new, more robust dataset (ca_hourly_demand.csv) manually from EIA: https://www.eia.gov/beta/states/states/ca/data/dashboard/electricity
- Added CO2 emissions (ca_co2_emissions_monthly.csv), started manually adding CA daily CO2 emissions (ca_co2_emissions_daily folder)
- Disaggregate electricty used for EV charging from other demands?

**10/20/22**:
- Ran into roadblocks, unclear direction for current project concept
- New abstract concept: assuming no change to energy sourcing, as CA hits different EV milestones, what is the expected increase in electricity demand needed and resulting emissions increase for these cars? Is it greater or less than current emissions from gas cars?

**11/16/22**:
- Hourly_demand_to_emissions, monthly_demand_to_emissions, etc. : exploratory notebooks. Analysis.ipynb contains all "final" data analysis relevant to final project & paper
- Updated abstract
- Added dataset sources to reference-list.MD: cumulative EV_sales, continuing to download ca_co2_emissions_daily datasets
- New analysis.ipynb and data_cleanup.ipnyb (compiled in all_data.csv)

**12/5/22**:
- Clean all files and rename
- Recap video submitted for class

**12/15/22**:
- Final paper
- Final commit