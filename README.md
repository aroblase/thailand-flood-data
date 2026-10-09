# Bangkok and Thailand Flood Risk Data, 2011-2026

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23260465.svg)](https://doi.org/10.5281/zenodo.23260465)

Flood data for Bangkok and Thailand compiled and cleaned by [ThaiFloodRisk.com](https://thaifloodrisk.com/en), from official Thai sources (Bangkok Metropolitan Administration, GISTDA) and open datasets. Free to reuse under [CC BY 4.0](LICENSE).

The interactive versions of these tables (maps, district reports, address checker) are on [thaifloodrisk.com](https://thaifloodrisk.com/en). The files are also available on the [open data page](https://thaifloodrisk.com/en/open-data), which always has the latest version.

## Files

All files are in [`data/`](data). Format: UTF-8 with BOM, comma-separated, one header row. Thai names are kept as published by the source.

| File | Rows | Content |
|---|---|---|
| [bangkok-street-flooding-episodes-2021-2026.csv](data/bangkok-street-flooding-episodes-2021-2026.csv) | 1,762 | Every standing-water episode recorded by the BMA on Bangkok's main roads |
| [bangkok-street-flooding-2021-2026.csv](data/bangkok-street-flooding-2021-2026.csv) | 50 | The same episodes by district and year |
| [bangkok-flooded-roads-2021-2026.csv](data/bangkok-flooded-roads-2021-2026.csv) | 26 | Bangkok's most flooded roads |
| [bangkok-flood-odds-by-forecast-rain.csv](data/bangkok-flood-odds-by-forecast-rain.csv) | 5 | Share of days with flooded roads by forecast rain |
| [bangkok-2011-flood-by-district.csv](data/bangkok-2011-flood-by-district.csv) | 154 | 2011 flood extent by district and sub-district |
| [bangkok-rail-stations-flood-risk.csv](data/bangkok-rail-stations-flood-risk.csv) | 189 | Flood risk of BTS, MRT and rail stations |
| [thailand-flood-risk-zones.csv](data/thailand-flood-risk-zones.csv) | 85 | Flood risk scores of districts, cities and destinations |

### bangkok-street-flooding-episodes-2021-2026.csv

Every standing-water episode recorded by the BMA Drainage and Sewerage Department on Bangkok's main roads, from 2 October 2021 to 2 October 2026: date, district, road (as published and normalized), location, depth (cm), verified duration (minutes) and rain recorded (mm). One row per episode. The 2026 records were rebuilt from the department's daily reports. Covers the main roads the BMA monitors, not minor streets. Interactive version: [Bangkok street flooding](https://thaifloodrisk.com/en/tools/bangkok-street-flooding).

### bangkok-street-flooding-2021-2026.csv

Street flooding episodes summed by district: total episodes, episodes per year (2021-2026), days with flooding, maximum depth (cm) and median duration (minutes) for each of the 50 districts.

### bangkok-flooded-roads-2021-2026.csv

The 26 roads with 20 or more episodes from October 2021 to October 2026: rank among all roads in the records, episodes, days, median and maximum depth (cm), median duration (minutes), median rain (mm), districts crossed and the most flooded spot. Road normalization and hotspot grouping by ThaiFloodRisk.com.

### bangkok-flood-odds-by-forecast-rain.csv

For each band of forecast daily rain over Bangkok (0-1, 1-5, 5-10, 10-20 and 20+ mm), the number of days since 2022, how many ended with at least one flooded main road recorded by the BMA, the share, and how many had 10 or more flooded places. Forecasts from the Open-Meteo forecast archive.

### bangkok-2011-flood-by-district.csv

Share of each of Bangkok's 50 districts and 154 sub-districts (khwaeng) inside the areas mapped under water by GISTDA in the 2011 flood, plus the district share flooded at least once from 2012 to 2024. One row per sub-district. Satellite radar reads water poorly between buildings, so dense riverside areas can read higher than what was observed on the ground. Interactive map: [Bangkok 2011 flood by district](https://thaifloodrisk.com/en/tools/bangkok-2011-flood-by-district).

### bangkok-rail-stations-flood-risk.csv

Flood risk of 189 BTS, MRT and rail stations: lines, coordinates, flood risk score, SRTM elevation (a surface model that includes buildings), BMA LiDAR ground elevation where available, years flooded in GISTDA satellite maps out of the years covered (2011-2024), and distance to the nearest canal or river. Interactive version: [Bangkok BTS and MRT stations](https://thaifloodrisk.com/en/tools/bangkok-bts-mrt-stations).

### thailand-flood-risk-zones.csv

Flood risk score of 85 zones (Bangkok's 50 districts, suburban districts, cities and destinations across Thailand) with its three factors: SRTM elevation (40%), years flooded in GISTDA satellite maps 2011-2024 (35%) and distance to the nearest canal or river (25%). Adds BMA LiDAR ground elevation and the number of sub-districts inside and outside BMA flood protection areas where available. Each row links to the zone's report on thaifloodrisk.com. See the [methodology](https://thaifloodrisk.com/en/methodology).

## Sources

- Bangkok Metropolitan Administration, Drainage and Sewerage Department (data.bangkok.go.th, dds.bangkok.go.th)
- GISTDA flood-frequency layer
- SRTM elevation via OpenTopoData; BMA LiDAR
- OpenStreetMap waterways (ODbL); Wikidata (stations)
- Open-Meteo forecast archive
- Sub-district boundaries: OpenGISData-Thailand

The original sources keep their own terms. The compilation, cleaning and scores are by ThaiFloodRisk.com.

## How to cite

> ThaiFloodRisk.com (2026). Bangkok and Thailand Flood Risk Data 2011-2026 [Data set]. Zenodo. https://doi.org/10.5281/zenodo.23260465. CC BY 4.0.

## Contact

Found an error? Open an issue, or write via [thaifloodrisk.com](https://thaifloodrisk.com/en).
