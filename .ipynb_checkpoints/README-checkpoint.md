# Vessel Operations Analysis – Profision Data Challenge

This project is part of a Quant Analyst internship assessment. It involves analyzing vessel tracking and characteristics data to extract insights about vessel behavior, cargo loading, and regional activity using Python and standard data libraries.

---

## Repository Structure

├── profision-vessel-analysis.ipynb # Main Jupyter Notebook with analysis, plots, and commentary
├── requirements.txt # Python dependencies used (generated via pip freeze)
├── data/ # Folder to store input CSV files
│ ├── vessel_positions.csv
│ └── vessel_characteristics.csv


---

## Objectives Covered

1. **Data Cleaning:** Loaded and cleaned vessel tracking and characteristics data. Documented missingness and unstructured fields.
2. **Exploratory Data Analysis (EDA):** Explored vessel status, AIS speed, and AIS draft distributions.
3. **Vessel Classification:** Created a new `vessel_class` attribute based on DWT and visualized vessel distribution.
4. **Cargo Analysis:** Analyzed cargo commodity groups by vessel class.
5. **Geographical Analysis:** Defined a Southeast Asia polygon and visualized vessels operating in the region.
6. **Deep Dive Analysis:**
   - Identified cargo loaded in Southeast Asia (Aug 20–24, 2024)
   - Identified the top 2 exports from each country
   - Highlighted top regional operators
   - Analyzed vessel loading via AIS vs design draft
   - Analyzed destination countries

---

## Tools & Libraries Used

- Python 3.11+
- Jupyter Notebook
- `pandas`, `numpy`, `matplotlib`, `seaborn`, `plotly`
- `shapely` (for polygon masking)
- `uv` (for managing virtual environments — bonus)

---

## How to Run

1. **Clone the Repository**
```bash
git clone https://github.com/halladaas/vessel-analysis.git
cd vessel-analysis
uv venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter notebook
```