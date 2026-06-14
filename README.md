# EMSC2010 – Week 3 Practical 2: Mapping with Cartopy

This repository contains the template Jupyter notebook for **Week 3 Practical 2** of *EMSC2010: Data Science for Earth System Scientists* at the Australian National University.

The session introduces **map-based visualisation** using `cartopy`, applied to global earthquake and tectonic plate boundary data.

---

## Notebook

### Notebook 1 – Plotting Earthquakes and Plate Boundaries (`NB1`)

**Dataset:** Global earthquakes with magnitude above 5 (longitude, latitude, magnitude, depth) and tectonic plate boundary coordinates, provided in `Earthquakes_and_Plates.xlsx`.

This notebook introduces `cartopy` for creating maps with different projections and overlaying geographic data. It covers:

- **Setting up Colab** — installing `cartopy` and its system dependencies (`libgdal-dev`, `libgeos-dev`, `libproj-dev`), which are not pre-installed in the Colab environment
- **Reading the data** — loading the earthquake (`EQ`) and plate boundary (`PB`) worksheets from the provided Excel file into separate `pandas` DataFrames
- **Global mapping** — building a global map using a **Robinson projection**, adding coastlines and continents, plotting earthquake locations as points coloured by magnitude, and overlaying tectonic plate boundaries as lines

The notebook then sets two open-ended mapping exercises for students to complete:

- Recreating the global map using a **Mercator projection** centred on a different longitude
- Creating a **regional map** (e.g. focused on Japan) using a `LambertConformal` projection with `ax.set_extent` to limit the map area

…and a final plotting exercise using the `subplot` skills from Week 3 Practical 1:

- A two-panel figure with a histogram of earthquake magnitude alongside a scatter plot of earthquake depth vs. magnitude

**Key concepts:** Map projections (Robinson, Mercator, Lambert Conformal), `cartopy` coordinate reference systems and map features, plotting geospatial point data, global vs. regional maps, histograms and scatter plots in subplots

**Libraries:** `pandas`, `matplotlib`, `cartopy`

> **Note:** The `Earthquakes_and_Plates.xlsx` data file must be uploaded to the Colab file space before running this notebook.

---

## Data Files

| File | Description |
|---|---|
| `Earthquakes_and_Plates.xlsx` | Global earthquake locations/magnitudes/depths (`EQ` sheet) and tectonic plate boundary coordinates (`PB` sheet) |

This file is included in the repository and must be uploaded to the Colab file space when running the notebook.

---

## Getting Started

This is a **template repository**. To begin working on the notebook:

1. Click **"Use this template"** at the top of this page to create a copy of the repository in your own GitHub account.
2. Open the notebook from your copy of the repository and click the **"Open in Colab"** badge at the top of the notebook to launch it in Google Colab.
3. Before submitting, replace the `uXXXXXXX` placeholder in the filename with your ANU student UID.

---

## Repository Structure

```
EMSC2010-W3-P2/
├── EMSC2010_W3_P2_NB1_uXXXXXXX.ipynb   # Plotting earthquakes and plate boundaries
├── Earthquakes_and_Plates.xlsx           # Earthquake and plate boundary data
├── LICENSE
└── README.md
```

---

## Course Information

| | |
|---|---|
| **Course** | EMSC2010 – Data Science for Earth System Scientists |
| **Institution** | Australian National University (ANU) |
| **Week** | 3 |
| **Session** | Practical 2 |
| **Topic** | Mapping with Cartopy |

---

## License

This repository is released under the [MIT License](LICENSE).
