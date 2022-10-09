**9/27/22**:

Submitted abstract proposal.

Continue finding literature on:
- Electricity consumption on California
- Approaches to electricity consumption prediction (regression...)
- EV electricity consumption
- California’s conventional car ban and its impacts

To do: find EV electricity consumption data

Added resources to /etc/reference-list.md


**10/5/22**:

Created main.py file
Added resources to /etc/reference-list.md
Added EV data, formatted all data in /src folder
-> CA_ec: current CA electricity consumption (predict over time)
-> CA_driven: total average miles driven in CA (predict over time)
-> avg_ev_ec: average EV electricity consumption, 0.2 kWh/km
-> proportion_ev: proportion of cars that are EVs (predict over time)
   
   simple equation: CA_ec_t + CA_driven_t * proportion_ev_t * avg_ev_ec

To calculate the amount of electricity consumed by EVs, do we take into account the exact models? i.e. 20% of sales are Tesla model Ys, 10% Nissan Leafs... which each have slightly different average kWh/km
-> taking the current average electricity consumption for EVs should be ok. Tesla sales are increasing, but overall, popular models have similar avg electricity consumption. If anything, as EV tech evolves, the average electricity consumption may go down, so using the current average will give us a slight overestimation.
-> after finishing this, try predicting major EV sales and taking them into account while calculating total EV energy consumption

Is just using proportion_ev accurate? Not all driver drive the same distance, i.e. kind of general consumer (family vs. single, urban vs. rural...), truck drivers, other specialty drivers

To do:
- Complete main.py (rename this maybe), generate predictions
- Look into distribution of types of drivers. Also, even after banning combustion engine sales, there will still be old gas cars around for a while
- perhaps I decided on too simple of a project; decide on further steps (elaborate on resulting data or include other factors in prediction) after completing initial proposal
