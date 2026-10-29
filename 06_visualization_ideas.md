# Future Visualization Ideas

These are **project ideas**, not already-built website features.

| Priority | Feature | Data source / input | Suggested presentation |
|---|---|---|---|
| High | Population by region | 2024 INE census | Choropleth map and ranked bars |
| High | Chile north-to-south | Coordinates and regional geography | Scrollable geographic journey |
| High | Astronomy facilities | Observatory locations and specifications | Interactive map and comparison table |
| High | Earthquake history | USGS / Chilean seismology | Timeline, magnitude chart, map |
| Medium | Climate zones | Meteorological records | Temperature and precipitation profiles |
| Medium | National parks | CONAF protected-area records | Filterable destination map |
| Medium | Chilean food | Curated cultural dataset | Regional food atlas |
| Medium | Copper production | Cochilco historical series | Annual time-series chart |
| Medium | Energy transition | Chilean energy ministry / CNE | Electricity-mix stacked chart |
| Medium | Tourism | Official visitor statistics | Seasonal trends and region comparison |

## Potential machine-readable datasets to add later

- `regions.csv`: region, population_2017, population_2024, area_km2, latitude, longitude
- `observatories.csv`: name, latitude, longitude, altitude_m, wavelength, instrument
- `earthquakes.csv`: date, magnitude_mw, latitude, longitude, depth_km
- `climate.csv`: station, year, month, temperature_c, precipitation_mm

## Primary data portals

- INE: https://www.ine.gob.cl/
- Census geographic viewer: https://visualizador.ine.gob.cl/
- Chilean open data: https://datos.gob.cl/
- USGS earthquake catalog: https://earthquake.usgs.gov/earthquakes/search/
- Cochilco: https://www.cochilco.cl/
- National Energy Commission: https://www.cne.cl/

## Next collection step

Add longer numeric time series with dates, units, downloadable source links and explicit missing-value markers. Avoid invented intermediate values.
