# Sarawak Mangrove Above-Ground Biomass (AGB) Field Data


The dataset provides above-ground biomass (AGB) estimates from 245 mangrove plots across Sarawak, Malaysia, collected between [month, year] and [month, year]. These measurements were used for training and validating machine learning models in combination with Sentinel-1 SAR and Sentinel-2 optical data.

---

## Contents
- **AGB_with_Coordinates.csv**  
  Plot-level AGB measurements with anonymised coordinates.

- **AGB_Summary_By_Species.csv**  
  Summary statistics (mean, SD, min, max) of AGB for each recorded mangrove species.

- **AGB_Plots_Assigned_Species.csv**  
  Species assignments for each plot, including common names and genus information.

---

## Data Description

### AGB_with_Coordinates.csv
| Column Name        | Description |
|--------------------|-------------|
| Plot_ID            | Unique plot identifier |
| Latitude           | Latitude in decimal degrees (rounded to 4 decimal places) |
| Longitude          | Longitude in decimal degrees (rounded to 4 decimal places) |
| Species            | Scientific name of dominant species in the plot |
| AGB_Mg_ha          | Above-ground biomass in megagrams per hectare (Mg ha⁻¹) |

### AGB_Summary_By_Species.csv
| Column Name        | Description |
|--------------------|-------------|
| Scientific_Name    | Scientific name of species |
| Genus              | Genus of the species |
| Common_Name        | Common name |
| Plot_Count         | Number of plots with this species |
| Mean_AGB_Mg_ha     | Mean AGB (Mg ha⁻¹) |
| SD_AGB_Mg_ha       | Standard deviation of AGB |
| Min_AGB_Mg_ha      | Minimum AGB |
| Max_AGB_Mg_ha      | Maximum AGB |

### AGB_Plots_Assigned_Species.csv
| Column Name        | Description |
|--------------------|-------------|
| Plot_ID            | Unique plot identifier |
| Scientific_Name    | Scientific name of assigned species |
| Common_Name        | Common name |
| Genus              | Genus |
| AGB_Mg_ha          | Above-ground biomass in Mg ha⁻¹ |

---

## Coordinate Reference System (CRS)
- **EPSG:4326** (WGS 84) – decimal degrees

---

## Data Collection Methodology
Plots of 30 m × 30 m were established to align with Sentinel-2 spatial resolution. Tree diameter at breast height (DBH) and height were measured for all stems ≥5 cm DBH. Species identification was conducted in the field. Above-ground biomass was estimated using species-specific or regionally validated allometric equations.

---

## Usage Notes
- Coordinates have been rounded to 4 decimal places (~11 m) to protect ecologically sensitive sites.
- Data can be joined with remote sensing imagery for calibration and validation of biomass models.
- Please cite the dataset if used in publications (see below).

---

## License
This dataset is released under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).

---

