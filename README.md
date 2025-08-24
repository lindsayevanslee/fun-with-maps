# Fun with Maps

Scripts for for extracting and visualizing geographic data from OpenStreetMap.

## Contents

- **`shapes_from_openstreetmap.ipynb`**: Jupyter notebook that demonstrates how to extract building outlines from OpenStreetMap using the `osmnx` library
- **`buildings_esrijson.csv`**: Sample output containing building names and their corresponding EsriJSON coordinate data

## Output
The main output is a CSV file with two columns:
- **`name`**: Building name from OpenStreetMap
- **`coordinates`**: EsriJSON format coordinates in the format: `{"rings": [[[longitude, latitude], ...]]}`

This format allows you to visualize these building outlines in Power BI with the ArcGIS visual

## Getting Started

1. **Install Dependencies**: Use the provided `environment.yml` to create a conda environment
   ```bash
   conda env create -f environment.yml
   conda activate fun-with-maps
   ```

2. **Run the Notebook**: Open `shapes_from_openstreetmap.ipynb` in Jupyter to explore building extraction

3. **Customize Location**: Change the `place` variable to extract buildings from any location worldwide

4. **Export for CSV**: The notebook automatically generates the CSV file ready for Power BI import

## Data Source
All building data is sourced from [OpenStreetMap](https://www.openstreetmap.org/), a collaborative project to create a free editable map of the world.
