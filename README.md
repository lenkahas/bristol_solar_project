# Calculating the solar potential for buildings in Bristol City, England, Part 2

A repository that shows how the Bristol Solar Team at the Open Data Bristol hackathon event (Nov 2018) estimated solar potential for buildings in Bristol and population potential for solar energy, England using open data (LiDAR - Environment Agency, Census) and open source tools (R,SAGA). 

This is second part of the analysis that has produced the estimates of solar irradiation and potential solar panel capacity and generation for buildings, street clusters, LSOAs and WARDs. Generalization of the estimates into 4 levels, helps to provide broader picture of the Bristol solar potential.

Additional, geodemographic open source data were used to provide population solar potential index. 

## Prerequisities

To run the code, you will need to have R installed. All required packages will be installed at the beginning of the rmarkdown. If you wish to use the data for analysis, we provide compressed folder simple CSVs for each layer as well as spatial .gpkg layer. Be aware of the geopackage format we used for exporting, it preserves the BNG projection and coordinates, so you can use any GIS software to preview the data and transform into different format, or use the [Bristol Open data]() to download formats such as GeoJSON or SHP.


## Authors

* **Tom Statham** - *Part 1:Calculating Solar Irridiance for Individual Buildings in Bristol,England using LiDAR* - [tastatham](https://github.com/tastatham)
* **Lenka Hasova** - *Part 2: Evaluating the potential for PV installations on building roofs* - [hasovalenka](https://github.com/hasovalenka)
* **David Saunders** - *For his domain knowledge of solar energy and project manager*  

## License

This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/tastatham/bristol_solar_project/blob/master/LICENSE.md) file for details

## Credits
[Ordnance Survey for OS Zoomstack Buildings](https://www.ordnancesurvey.co.uk/business-and-government/licensing/using-creating-data-with-os-products/os-opendata.html).
[Environment Agency for LiDAR DSM 1m](https://www.ordnancesurvey.co.uk/business-and-government/licensing/using-creating-data-with-os-products/os-opendata.html).
[Office for National Statistics](https://www.ons.gov.uk/census/2001censusandearlier/dataandproducts/copyrightandlicensing/licenseinformation)
[Consumer Data Research Centre](https://www.cdrc.ac.uk/data-services/cdrcdata/)
[Energy Performance of Buildings Data England and Wales](https://epc.opendatacommunities.org/docs/copyright)

## Acknowledgments

* We would like to thank Bristol City Council for the small stipend for carrying out this work.

## Attachments

| Variable description                                   | Shortcut used within data|
|:-------------------------------------------------------|-------------------------:|
|ID                                                      | ID                       |
|Total roof area (m2)                                    | 1_TRA                    |
|Incoming radiation (kWh/per annum)                      | 2_IRTRA                  |
|Unshaded roof area (m2)	                               | 3_URA                    |
|Incoming radiation on unshaded roof area (kWh/per annum)| 4_IRURA                  |
|Potential number of panels/ panel capacity (kWh)        | 5_PNP                    |
|Potential PV system generation (kWh/per annum)	         | 6_PPVSG                  |
|CO2 savings (kg/per annum)                              | 7_CO2S                   |
|Money savings (£/per annum)                             | 8_MS                     |
|LSOA11CD	                                               | LSOA11CD                 |
|IMD Score (The higher the number, the more deprived)    | 9_IMD                    |
|Probability of meeting homeowner (1 low - 15 high)	     | 10_PMH                   |
|Population potential for Solar energy (1 low - 5 high)	 | 11_PPS                   |
|Existing panels capacity (kWh)	                         | 12_EPC                   |
|Difference between potential and existing capacity	     | 13_DPEC                  |
