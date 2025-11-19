# Urban Heat Island Analysis — Phoenix, AZ

Spatial Data Science repo exploring urban heat islands, vegetation health, and social vulnerability in Phoenix, Arizona, using satellite and census data.

---

![Phoenix Heat Islands Map](figures/choropleths/phoenix_heat_islands.png)
*Example map output; see the `figures/` folder for more*

---

## Quick Start

1. **Clone the repository**
git clone https://github.com/fran-salas/urban-heat-island-analysis.git
cd urban-heat-island-analysis



2. **Set up your Python environment**
python -m venv venv
venv\Scripts\activate # On Windows Command Prompt
pip install --upgrade pip
pip install -r requirements.txt



3. **Add your Census API key**
- Request your key: [census.gov/data/key_signup.html](https://api.census.gov/data/key_signup.html)
- Copy `.env.example` to `.env` and add your key

4. **Obtain raw data sources**
- Detailed links and instructions: [`data/raw/DATA_SOURCES.md`](data/raw/DATA_SOURCES.md)
- Place downloaded files in the `data/raw/` folder

5. **Verify the setup**
python verify_environment.py
python test_census_api.py



---

## Repository Structure

urban-heat-island-analysis\
│
├── data\
│ ├── raw\
│ └── processed\
├── src\
├── notebooks\
├── figures\
│ ├── choropleths\
│ ├── moran_plots\
│ └── lisa_maps\
├── tests\
├── docs\
│ ├── methodology.md\
│ ├── findings.md\
│ └── data_strategy.md\
├── .env.example\
├── requirements.txt\
├── environment.yml\
└── README.md



---

## Data Sources

- Phoenix boundary: [City Open Data Portal](https://phoenixopendata.com)
- Census tracts and ACS variables: [US Census Bureau](https://www.census.gov/data.html)
- Satellite imagery: [USGS EarthExplorer](https://earthexplorer.usgs.gov)
- Full instructions: [`data/raw/DATA_SOURCES.md`](data/raw/DATA_SOURCES.md)

---

## Analysis Pipeline

- Exploratory spatial analysis, statistical mapping, and autocorrelation
- Detection of heat island clusters using Global Moran’s I and LISA
- Band operations for NDVI and vegetation mapping
- Socioeconomic overlays for vulnerability analysis
- Notebook code follows a real workflow approach—professional, somewhat messy, not over-polished

---

## Security & API Keys

- Store API keys in `.env` (private, never committed)
- Use `.env.example` for templates and onboarding
- For security details and tips, see [`docs/API_KEY_SECURITY.md`](docs/API_KEY_SECURITY.md)

---

## Documentation

- Methodology: [`docs/methodology.md`](docs/methodology.md)
- Findings: [`docs/findings.md`](docs/findings.md)
- Data strategy: [`docs/data_strategy.md`](docs/data_strategy.md)

---

## Contact

Lead: Francisco Salas Gomez  
Email: [francisco.salasgomez@outlook.com](mailto:francisco.salasgomez@outlook.com)  
GitHub: [fran-salas](https://github.com/fran-salas)

For issues or collaboration ideas, please use [GitHub Issues](https://github.com/fran-salas/urban-heat-island-analysis/issues).

---

*MIT License • 2025*