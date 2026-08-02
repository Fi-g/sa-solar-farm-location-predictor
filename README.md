# South African Solar Farm Location Predictor

A data science portfolio project identifying optimal solar farm locations for underserved rural communities across South Africa.

## Project Overview

This project combines village-level settlement data, national grid performance data, and weather station observations to:

- Score 76941 South African settlements for solar farm suitability
- Forecast national electricity demand through to 2030
- Identify 8 priority solar farm locations across 3 provinces
- Calculate the minimum number of farms needed to reach 25% renewable energy penetration by 2030

## Dashboard

View the interactive dashboard here: 
[SA Solar Farm Location Predictor Dashboard](https://app.powerbi.com/reportEmbed?reportId=01f21b25-a0c3-48bb-884c-c4994c7f19f5&autoAuth=true&ctid=cf87d705-23dc-4ae8-a866-47fb4924fa7a)

Or view the static PDF export:
[Dashboard PDF](outputs/SA_Solar_Dashboard.pdf)

## Key Findings 

- Thabazimbi (Limpopo) ranks as the top priority location, serving 108202 people within its 50km transmission radius
- The Northern Cape dominates suitability ranking due to high solar irradiance, low cloud cover, and low security risk
- A minimum of 221 solar farms are needed by 2030 to reach the 25% RE penetration target
- South Africa's grid demand has declined consistently since 2021 due to accelerating rooftop solar adoption

## Project Structure

| Folder | Description |
|---|---|
| notebooks / | Jupyter notebooks for each project phase |
| dashboard / | Power BI dashboard (.pbix) |
| report/ | Full portfolio report |
| outputs/ | Visualisation files (PNG and HTML) |
| data/ | Raw and processed data (not included - see Data Sources) |

## Data Sources 
| Dataset | Source | Access |
|---|---|---|
| National grid data | Eskom | Formal data request |
| Weather station data | South African Weather Service (SAWS) | Formal data request |
| Settlement data | DRE Atlas | https://energydata.info/dataset/south-africa-distributed-renewable-energy-dre |

## Tools and Technologies 

Python | SQL | SQLite | Power BI | Prophet | GeoPandas | Folium

## Notebooks 

| Notebook | Description |
|---|---|
| phase1_eskom_data_cleaning | Eskom dataset cleaning |
| phase1_saws_data_parsing | SAWS Excel parsing |
| phase1_saws | SAWS SQL cleaning |
| phase1_settlements_data_cleaning | Settlement dataset cleaning |
| phase2_settlements_saws | Spatial joining and dataset merging |
| phase3_visualisations | All EDA and analystical visualisations |
| phase3_time_series | Prophet demand forecasting model |
| phase4_geospatial_analysis | Solar suitability scoring model |
| phase5_optimisation | Minimum farm count optimisation |
| phase6_sample | Sampling and file type conversions |

## Author 

Refiloe Ntshabele |
Second Year Data Science Student |
www.linkedin.com/in/refiloe-ntshabele

## Licence 

This project is for portfolio purposes. Data files are not included due to data request aggrements with Eskom and SAWS.
