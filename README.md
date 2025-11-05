# GeoVision Pro - Advanced GIS Topology Analysis Tool

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![GeoPandas](https://img.shields.io/badge/GeoPandas-0.12%2B-green)
![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20Linux%20%7C%20MacOS-lightgrey)

A professional desktop application for advanced GIS topology analysis, correction, and spatial data processing. Built with Python and modern geospatial libraries.

## Features

### Data Import & Processing
- **Multi-format Support**: SHP, GeoJSON, GPKG, KML, CSV
- **CSV to Spatial Conversion**: Convert tabular data to points or convex hulls
- **Coordinate Reference Systems**: Support for 13+ CRS including WGS84, Web Mercator, UTM zones
- **Real-time Reprojection**: On-the-fly coordinate transformation

### Advanced Topology Analysis
- **Gap Detection**: Identify empty spaces between polygons
- **Overlap Detection**: Find overlapping polygon areas
- **Sliver Detection**: Locate very small/thin polygons
- **Connectivity Validation**: Check network connectivity for lines
- **Duplicate Vertices**: Detect duplicate coordinate points
- **Self-Intersections**: Find invalid self-intersecting geometries
- **Comprehensive Checks**: Run all applicable topology analyses

### Topology Correction
- **Automated Fixing**: One-click topology correction
- **Customizable Tolerance**: Adjustable snap tolerance (0.0001 - 0.1)
- **Smart Algorithms**: Proper overlap resolution, geometry snapping, invalid geometry repair
- **Validation**: Post-correction validation and reporting

### Visualization & Export
- **Interactive Maps**: Modern dark theme visualization
- **Error Highlighting**: Color-coded topology errors
- **Data Preview**: Tabular data inspection
- **Multiple Export Formats**: GeoJSON, Shapefile, GPKG, CSV
- **Results Export**: Save analysis reports as text files

## Installation

### Prerequisites
- Python 3.8 or higher
- Git

### Quick Install (Recommended)
```bash
# Clone the repository
git clone https://github.com/yourusername/geovision-pro.git
cd geovision-pro

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run the application
python main.py
```

### Manual Installation
```bash
pip install geopandas pandas matplotlib tkinter shapely
python main.py
```

### Requirements
```txt
geopandas>=0.12.0
pandas>=1.5.0
matplotlib>=3.6.0
shapely>=2.0.0
numpy>=1.21.0
```

## Usage

### Loading Data
1. Click **Browse** to load spatial files (SHP, GeoJSON, GPKG) or CSV files
2. For CSV files, select X and Y coordinate columns
3. Choose appropriate Coordinate Reference System

### Data Processing
- **Convert CSV**: Transform tabular data to spatial points
- **Create Convex Hull**: Generate polygon from point clusters
- **Reproject Data**: Transform between coordinate systems

### Topology Analysis
1. Set **Snap Tolerance** for precision control
2. Select analysis options (overlaps, gaps, invalid geometries, etc.)
3. Click **Analyze Topology** to run comprehensive checks
4. View results in the **Results Tab**

### Topology Correction
1. Configure correction options in the sidebar
2. Click **Fix Topology** to apply automated corrections
3. Review validation results in the processing log

### Export Results
- Choose export format (GeoJSON, Shapefile, GPKG, CSV)
- Click **Export Processed Data** to save corrected data
- Use **Export Results** to save analysis reports

## Technical Details

### Core Technologies
- **Backend**: Python, GeoPandas, Shapely, Pandas
- **GUI**: Tkinter with ttk widgets
- **Visualization**: Matplotlib with custom theming
- **Spatial Operations**: GEOS, PROJ, GDAL

### Topology Algorithms
- **Overlap Resolution**: Priority-based polygon differencing
- **Geometry Snapping**: Shapely's snap function with configurable tolerance
- **Validation**: Comprehensive post-processing validation
- **Error Handling**: Robust exception handling

### Supported CRS Systems
- WGS84 (EPSG:4326)
- Web Mercator (EPSG:3857)
- UTM Zones 10N-19N (EPSG:32610-32619)
- British National Grid (EPSG:27700)

## Contributing
We welcome contributions! Please see our Contributing Guidelines for details.

### Development Setup
```bash
git clone https://github.com/Sammaglin/geovision-pro.git
cd geovision-pro
pip install -r requirements-dev.txt
```

## Acknowledgments
- **GeoPandas** team for excellent geospatial data handling
- **Shapely** library for robust geometric operations
- **Matplotlib** for powerful visualization capabilities

## Support
- **Email**: sammaglin1971@gmail.com

---

**⭐ If you find this project useful, please give it a star on GitHub!**

---
