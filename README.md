# Michigan PFAS Data Dashboard 🧪🌊

![GitHub last commit](https://img.shields.io/github/last-commit/Nancy-Odhiambo/Michigan-PFAS-Data)
![GitHub issues](https://img.shields.io/github/issues/Nancy-Odhiambo/Michigan-PFAS-Data)
![GitHub license](https://img.shields.io/github/license/Nancy-Odhiambo/Michigan-PFAS-Data)

---

## Introduction 📖
Per- and polyfluoroalkyl substances (PFAS) are a large group of man-made chemicals, including perfluorooctanoic acid (PFOA) and perfluorooctanesulfonic acid (PFOS). These chemicals have been widely used in manufacturing, firefighting, and consumer products. Because PFAS are highly persistent in the environment and in the human body, they can accumulate over time and pose potential health risks.

PFAS contamination in Michigan has raised significant public health and environmental concerns, echoing past environmental advocacy efforts such as those led by Erin Brockovich. This project aims to make PFAS-related data more accessible and easier to explore through an interactive dashboard.

The dashboard allows users to visualize PFAS concentrations in surface water, public water supplies, and known contamination sites across Michigan. By improving access to PFAS data, we hope to support research, policy discussions, and public awareness.

---

## Dashboard 🖥️
🔗 **[View the Live Dashboard Here](#)**  
*(View once ready)*

---

## Key Features ✨
- 🗺️ Interactive maps showing PFAS contamination sites across Michigan
- 🌊 Visualizations of PFAS concentrations in surface water
- 💧 Visualizations of PFAS levels in municipal drinking water
- 📊 Searchable tables and downloadable data
- 👥 User-friendly design to support researchers, policymakers, and the general public
*(To update with actual viasualizations)*
---

## Data Source 📂
This project uses publicly available PFAS datasets provided by the **Michigan Department of Environment, Great Lakes, and Energy (EGLE)** and the **Michigan PFAS Action Response Team (MPART)**.

- [Surface Water Sampling Data](https://gis-egle.hub.arcgis.com/datasets/egle::pfas-surface-water-sampling/about)
- [Public Water Supply Sampling Data](https://gis-egle.hub.arcgis.com/search?q=pfasgis)
- [Michigan PFAS Sites Data](https://www.michigan.gov/pfasresponse/investigations/sites-aoi)
- [PFAS Laboratory Analyte List (PDF)](https://www.michigan.gov/pfasresponse/-/media/Project/Websites/PFAS-Response/Sampling-Guidance/Minimum-Laboratory-Analyte-List.pdf?rev=a35aba56ec5a4922b986f01e25c1a19d&hash=04E6F164AA5F5CD29B83B39983341345)

<details>
<summary>📝 Surface Water Sampling Data Dictionary</summary>

| Variable | Description |
|----------|-------------|
| geoid | Geographic region ID (first 2 digits = state FIPS, last 3 = county FIPS) |
| longitude | Longitude of sampling location |
| latitude | Latitude of sampling location |
| lab_sample_id | Sample ID provided by analytical laboratory |
| site_code | Sampling location name |
| coc_sample_id | Sample ID listed on chain of custody |
| sample_type | Expanded description of type of sample collected |
| lab_name | Name of analytical laboratory |
| lab_job_name | Analytical laboratory's job/work order name |
| collection_date | Date sample was collected |
| analysis_method | Analysis method used |
| dilution_factor | Dilution factor used during sample prep |
| analysis_date | Date analysis was conducted |
| duplicate | Description of duplicate sample |
| watershed | Watershed sample collected from |
| waterbody | Waterbody sample collected from |
| location_code | Sampling location code |
| huc10 | 10-digit hydrological unit code |
| huc8 | 8-digit hydrological unit code |
| project | Associated project |
| description | Description of sampling location |
| additional_description | Additional description of sampling location |
| visit_id | ID of sampling event |
| sample_depth | Sampling depth |
| analyte | PFAS analyte |
| analyte_value | Analyte concentration (ppt/ng/L) |

</details>

<details>
<summary>💧 Public Water Supply Sampling Data Dictionary</summary>

| Variable | Description |
|----------|-------------|
| geoid | Geographic region ID (state + county FIPS) |
| longitude | Longitude of sampling location |
| latitude | Latitude of sampling location |
| system_name | Name of water supply system |
| system_type | Type of water supply system |
| sample_date | Date sample was collected |
| lab_name_code | Code for processing lab |
| analyte | PFAS analyte |
| analyte_value | Analyte concentration (ppt/ng/L) |

</details>

<details>
<summary>☢️ PFAS Sites Data Dictionary</summary>

| Variable | Type | Description |
|----------|------|-------------|
| geoid | double | Geographic region ID (state + county FIPS) |
| longitude | double | Longitude of sample location |
| latitude | double | Latitude of sample location |
| facility | character | Name of site |
| county | character | County of site |
| address | character | Physical address of site |
| city | character | City of site |
| zip_code | double | Zip code of site |
| type | character | Kind of site |
| residential_wells_sampled | character | Indicates if residential wells sampled (Yes/No/TBD/N/A) |
| site_lead | character | Contact person |
| site_lead_email | character | Contact email |
| site_lead_phone | character | Contact phone |
| hyperlink | character | Web link to site investigation summary |
| location | character | Geographic location description |
| military | character | Indicates if site is associated with military |
| facility_date | character | Date site published on MPART website |
| site_background | character | Background info on site |
| drinking_water_information | character | Info about drinking water quality and safety |
| anticipated_activities | character | Planned or upcoming state activities |

</details>

---

## Technologies Used 🛠️
- **Frontend:** Leaflet, Plotly (To update with actuals)
- **Backend:** R, Quarto, Markdown
- **Hosting:** GitHub Pages

---

## Attribution & Licensing 📜
- **Data Providers:** Michigan Department of Environment, Great Lakes, and Energy (EGLE); Michigan PFAS Action Response Team (MPART)  
  *Note: This dashboard is an independent project and is not affiliated with or endorsed by MPART or the State of Michigan.*

- **Project License:** The code for this project is licensed under the [MIT License](LICENSE)

- **Acknowledgments:** This project was created by **Nancy Odhiambo** as part of a Master's Graduate Research Assistantship in the **Department of Statistics, Grand Valley State University**.  
  Faculty Mentor: **Dr. Andrew DiLernia**
