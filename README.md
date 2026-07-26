# 🚶 The 15-Minute City: Walking Access in Liverpool

Can everyone in Liverpool reach a doctor, a school, a park, or a shop within a 15-minute walk — and does that depend on how deprived their neighbourhood is?

This project measures real walking access across Liverpool and compares it against deprivation data to see whether the city's most "walkable" idea holds up equally everywhere.

## What it does

1. **Builds Liverpool's actual walking network** from OpenStreetMap — every street, footpath, and pedestrian crossing — using OSMnx.
2. **Calculates walking isochrones**: for points across the city, it works out exactly how far someone can walk in 5, 10, and 15 minutes, following real streets (not just "as the crow flies").
3. **Finds nearby services**: healthcare, schools, food shops, green space, and cultural venues within each walkshed.
4. **Overlays deprivation data** (the government's Index of Multiple Deprivation) to see whether the most deprived neighbourhoods are also the least walkable.
5. **Builds an interactive dashboard** to explore any neighbourhood's 15-minute access for yourself.

## Key finding

Physical closeness to amenities doesn't guarantee access — some deprived areas have services nearby "on paper" but poor street connectivity means real walking times are much longer.

## Try it yourself

- **`liverpool_15min_city.ipynb`** — the full analysis, step by step
- Open the notebook and run the final cells for the interactive neighbourhood explorer

## Built with

`Python` · `OSMnx` · `NetworkX` · `GeoPandas` · `Folium` · `Panel` · OpenStreetMap · UK Index of Multiple Deprivation (IMD)

## Run it locally

```bash
pip install osmnx geopandas pandas numpy networkx matplotlib folium panel requests
jupyter notebook liverpool_15min_city.ipynb
```

Run all cells top to bottom — it downloads live street network and deprivation data, so it needs an internet connection.
