# ML-Climate-Project-Template-Fall2022

- The file `abstract.md` contains the original project proposal and the formal abstract contained in the final paper document.
- The file `journal.md` is a diary of progress over the course of the semester.
- The `doc/` directory contains the LaTeX document and PDF file for the final paper.
- The `src/` directory contains the data analyzed through this project as well as Notebooks documenting these analyses.
- The `etc/` directory contains additional documentation, a single file containing resources and notes for myself throughout the project, less formal than the journal.

**Data sources**
See final paper for formal references.
1) California Independent System Operator: ca_daily_demand, ca_daily_emissions, ca_daily_renewables, ca_daily_supply folders; ca_monthly_emissions.csv\
2) National Centers for Environmental Information: all_states_monthly_max_temp.csv, all_states_monthly_min_temp.csv, all_sates_monthly_precip.csv\
3) US Energy Information Administration: ca_hourly_demand.csv, ca_monthly_supply.csv\
4) Argonne: usa_monthly_car_sales.csv\
Cleaned data:
- minute_emissions_demand_resources.csv: derived from 1
- monthly_demand.csv: derived from 3
- monthly_precip.csv, monthly_tmin.csv, monthly_tmax.csv: derived from 2
- monthly_vehicles: derived from yearly_vehicles_reformat.csv and 4)