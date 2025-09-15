# Michigan PFAS Data

## Description  

From the state of Michigan's website:  

PFAS are a large group of man-made chemicals that include **perfluorooctanoic acid (PFOA)** and **perfluorooctanesulfonic acid (PFOS)**. PFAS have been used globally during the past century in manufacturing, firefighting, and thousands of common household and consumer products. These chemicals are persistent in the environment and in the human body — meaning they don't break down and can accumulate over time.  

In recent years, experts have become increasingly concerned about the potential effects of high concentrations of PFAS on human health.  

PFAS contamination in West Michigan has unfortunately made headlines, reminiscent of other environmental advocacy efforts like that of renowned whistleblower Erin Brockovich.  

---

There are multiple PFAS-related data sets available from the state of Michigan contained in a single zipped file:  
➡️ [pfas_data.zip](https://github.com/dilernia/STA418-518/blob/main/Data/pfas_data.zip)  

Datasets included:  
- **Surface water sampling data**: PFAS concentrations in surface water samples 🏞🐟  
- **Public water supply sampling data**: PFAS concentrations in municipal drinking water samples 💧  
- **PFAS sites data**: PFAS contamination or investigation sites ☢️  

Additional resources:  
- [Surface water data dictionary](https://gis-egle.hub.arcgis.com/datasets/egle::pfas-surface-water-sampling/about)  
- [Minimum Laboratory Analyte List (EGLE, HHS, MDARD, DNR)](https://www.michigan.gov/pfasresponse/-/media/Project/Websites/PFAS-Response/Sampling-Guidance/Minimum-Laboratory-Analyte-List.pdf?rev=a35aba56ec5a4922b986f01e25c1a19d&hash=04E6F164AA5F5CD29B83B39983341345)  

---

## Source  

Data was obtained from the [State of Michigan GIS Hub](https://gis-egle.hub.arcgis.com/search?q=pfasgis).  

---

## Data Dictionary  

### Surface Water Sampling Data  

| Variable                | Description                                                                 |
|--------------------------|-----------------------------------------------------------------------------|
| geoid                   | Geographic region ID (first 2 digits = state FIPS, last 3 digits = county) |
| longitude               | Longitude coordinate of sampling location                                   |
| latitude                | Latitude coordinate of sampling location                                    |
| lab_sample_id           | Sample ID provided by the analytical laboratory                            |
| site_code               | Sampling location name                                                      |
| coc_sample_id           | Chain-of-custody sample ID provided to laboratory                          |
| sample_type             | Description of sample type collected                                       |
| lab_name                | Analytical laboratory name                                                  |
| lab_job_name            | Analytical laboratory job/work order name                                   |
| collection_date         | Date sample was collected                                                   |
| analysis_method         | Method used by laboratory for analysis                                      |
| dilution_factor         | Dilution factor applied during sample prep                                 |
| analysis_date           | Date laboratory conducted analysis                                          |
| duplicate               | Duplicate sample description                                               |
| watershed               | Watershed of collection site                                                |
| waterbody               | Waterbody of collection site                                                |
| location_code           | Sampling location code                                                      |
| huc10                   | 10-digit hydrological unit code                                             |
| huc8                    | 8-digit hydrological unit code                                              |
| project                 | Associated project name                                                     |
| description             | Description of sampling location                                            |
| additional_description  | Additional details of sampling location                                     |
| visit_id                | Sampling event ID                                                           |
| sample_depth            | Depth at which sample was collected                                         |
| analyte                 | PFAS analyte name                                                           |
| analyte_value           | PFAS analyte concentration (parts per trillion, ppt or ng/L)               |  

---

### Public Water Supply Sampling Data  

From EGLE:  

The dataset includes information from both the State of Michigan–funded PFAS drinking water sampling effort and ongoing compliance monitoring. Each location may have multiple samples across different dates.  

| Variable        | Description                                                                 |
|-----------------|-----------------------------------------------------------------------------|
| geoid           | Geographic region ID (FIPS: state + county)                                |
| longitude       | Longitude of sampling location                                              |
| latitude        | Latitude of sampling location                                               |
| system_name     | Water supply system name                                                   |
| system_type     | Water supply system type                                                   |
| sample_date     | Date of sample collection                                                  |
| lab_name_code   | Processing lab code                                                        |
| analyte         | PFAS analyte                                                               |
| analyte_value   | PFAS analyte concentration (ppt or ng/L)                                   |  

---

### PFAS Sites  

_Last updated: 02/05/2025_  
_Downloaded: 02/25/2025_  

➡️ Cleaned CSV: [pfas_sites.csv](https://raw.githubusercontent.com/dilernia/STA418-518/refs/heads/main/Data/pfas_sites.csv)  

From EGLE: The Michigan PFAS Sites layer is the official list of PFAS sites in the state. Data is updated as new PFAS sites are identified.  

| Variable                   | Type     | Description                                                                 |
|-----------------------------|----------|-----------------------------------------------------------------------------|
| geoid                      | double   | Geographic region ID (FIPS: state + county)                                |
| longitude                  | double   | Longitude coordinate of sample location                                    |
| latitude                   | double   | Latitude coordinate of sample location                                     |
| facility                   | character| Name of the site                                                            |
| county                     | character| County name                                                                |
| address                    | character| Physical address of project site                                           |
| city                       | character| City of site location                                                      |
| zip_code                   | double   | Zip code of site                                                           |
| type                       | character| Type of site                                                               |
| residential_wells_sampled  | character| Whether residential wells were/are sampled (Yes/No/TBD/N/A)                |
| site_lead                  | character| Site contact person                                                         |
| site_lead_email            | character| Site contact email                                                          |
| site_lead_phone            | character| Site contact phone                                                          |
| hyperlink                  | character| URL to investigation summary                                               |
| location                   | character| Geographic location description                                            |
| military                   | character| Whether site is military-related                                           |
| facility_date              | character| Date site published on MPART website                                       |
| site_background            | character| Background information                                                     |
| drinking_water_information | character| Drinking water safety information                                          |
| anticipated_activities     | character| Planned or upcoming state activities                                       |  

---

## License  

This project is released under the **xxxx**.  
