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
| LONG (longitude) – geographic longitude (decimal degrees) |

## 3. DATASET 2: ADMINISTRATIVE BOUNDARIES (SHAPEFILE)
