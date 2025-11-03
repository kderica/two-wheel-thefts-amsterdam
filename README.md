## Amsterdam Bike Theft Analysis

A small data project analyzing reported bicycle thefts in Amsterdam, with an emphasis on 2024 and recent-year trends. It includes a Jupyter notebook for analysis and a generated interactive map.

### Repository contents
- `analysis.ipynb`: Main notebook used to clean, analyze, and visualize the data.
- `2024_bikes.csv`: Bike theft counts for 2024 by Amsterdam neighborhood/buurt. 
- `last_4_years.csv`: Bike theft counts (city and neighborhoods) across multiple recent years.
- `INDELING_BUURT.csv`: Amsterdam neighborhood (buurt) reference with codes, names, centroids, and polygons.
- `amsterdam_bike_thefts_2024.html`: Interactive Leaflet/Folium map generated from the notebook.

### Quick start
1. Create and activate a Python environment (Python 3.9+ recommended).
2. Install dependencies:

```bash
pip install pandas numpy folium jupyter matplotlib
```

3. Launch Jupyter and open the notebook:

```bash
jupyter notebook analysis.ipynb
```

4. Run all cells to reproduce the analysis and generate outputs (including the interactive map HTML).

### Viewing the interactive map
- Open `amsterdam_bike_thefts_2024.html` in a web browser to explore the 2024 bike theft distribution by neighborhood.

### Data notes
- The CSV files use semicolon delimiters and quoted headers/values.
- The counts represent registered incidents ("Geregistreerde misdrijven (aantal)").
- Neighborhood names and codes in `INDELING_BUURT.csv` can be used to join geographic shapes to metrics for mapping.

### Reproducibility
- If you modify the notebook, re-run it to refresh `amsterdam_bike_thefts_2024.html`.
- Ensure the CSV files remain in the project root or update paths inside the notebook accordingly.

### Data sources
- `2024_bikes.csv` and `last_4_years.csv`: obtained from the Police Open Data portal using different filters, then cleaned (including some manual cleaning): https://data.politie.nl/#/Politie/nl/dataset/47018NED/table?ts=1762120143951
- `INDELING_BUURT.csv`: neighborhood geometries and attributes from the Municipality of Amsterdam open geodata: https://maps.amsterdam.nl/open_geodata/


# two-wheel-thefts-amsterdam
