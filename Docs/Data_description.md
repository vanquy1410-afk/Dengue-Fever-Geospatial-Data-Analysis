## DATA DESCRIPTION

# 1.Overview
This project uses epidemiological and spatial data to analyze the distribution of Dengue Fever cases in Nha Trang City, Viet Nam. The datasets support spatial analysis and visualization in QGIS.
The data is designed for spatial analysis and visualization using GIS tools.

---

## 2. DATASET 1: DENGUE CASES (EXCEL)

**File name:** `SXHD2022_NhaTrang.xlsx`  
**Format:** Excel (.xlsx)

### 2.1 Description
This dataset contains reported dengue fever cases with associated geographic coordinates. It is used to generate point layers and support density-based spatial analysis. 


### 2.2 Key Fields
The original Excel file contains additional attributes. However, for the purpose of this project, only Case ID and coordinate fields are required for this GIS analysis.

The analysis focuses exclusively on:
| Column Name | Description |
|------------|------------|
| Mã số (case_id) | Unique identifier for each dengue case |
| LAT (latitude) | Geographic latitude (decimal degrees) |
| LONG (longitude) | Geographic longitude (decimal degrees) |

---

## 3. DATASET 2: ADMINISTRATIVE BOUNDARIES (SHAPEFILE)

**File name:** `BanDoXaVN_UTM`  
**Format:** ESRI Shapefile  
**Geometry type:** Polygon  
**Data origin:** Derived Dataset  


### 3.1 Included Files

- `BanDoXaVN_UTM.shp` – Geometry
- `BanDoXaVN_UTM.shx` – Shape index
- `BanDoXaVN_UTM.dbf` – Attribute table
- `BanDoXaVN_UTM.prj` – Coordinate reference system

### 3.2 Source Data

The original dataset is a nationwide commune/ward-level administrative boundary shapefile of Viet Nam.

### 3.3 Data Preparation

The dataset used in this project was derived by extracting and filtering administrative units belonging to Nha Trang City from the national-level shapefile.

The processing steps include:

- Selecting features where the administrative unit belongs to Nha Trang City.
- Exporting selected features as a separate shapefile.
- Preserving original geometry and attribute structure.

### 3.4 Description
This dataset represents ward-level administrative boundaries of Nha Trang City. It is used for spatial joins, aggregation, and thematic mapping.

### 3.5 Coordinate Reference System (CRS)
- EPSG: 3406  
- Datum: VN-2000 /UTM Zone 49N

---

## 4. DATA USAGE
The datasets are used for:
- Point mapping of dengue cases.
- Density Estimation (Heatmap).
- Spatial aggregation by administrative wards.
- Exploratory spatial data analysis in QGIS.

---

## 5. TOOLS
- QGIS – Spatial analysis and visualization.
- Microsoft Excel – Data cleaning and preprocessing.

---

## 6. DATA LIMITATIONS
- Possible inaccuracies in reported coordinates.
- Temporal coverage depends on the reporting period.
- Case aggregation level may vary depending on the data source.
