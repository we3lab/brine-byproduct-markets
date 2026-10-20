# Spatiotemporal demand and price data for valorized constituents from U.S. brines
### Caroline E. Adkins and Meagan S. Mauter
*Note: The manuscript supported by this repository is currently under review.*

The United States generates approximately 1 trillion gallons of brine each year. Although these brines are typically managed as waste streams, they contain diverse ions and compounds of value as industrial feedstocks. Brine valorization, defined as the recovery and sale of these constituents, could offset disposal costs and enhance the sustainability of domestic supply chains. The low market value of most materials derived from brine constituents, however, means that the success of valorization depends on local demand for, and prices of, these products. This dataset provides this essential market context by quantifying annual state-level demand and national prices for 16 byproducts recoverable from U.S. brines for a five year period from 2021 to 2025. We systematically obtain raw data on byproduct end-use markets, domestic consumption, and the spatial distribution of relevant industries from government, industry, and market research sources, and we validate the results against external benchmarks. The resulting dataset enables feasibility assessments of brine valorization in the U.S. that explicitly account for spatiotemporal market constraints.

# Table of Repository Contents

### `data_processing/`
| File | Description |
|------|-------------|
| `01_demand_calculations.ipynb` | Calculates annual state-level demand for each byproduct using raw market data and spatial disaggregation proxies |
| `02_validation.ipynb` | Internal consistency checks and external benchmark validation of demand estimates |
| `03_visualization.ipynb` | Figure generation and other visualizations |

### `data/inputs/`
| File | Description |
|------|-------------|
| `sw1_demand.xlsx` | Raw market share, national demand, and price data by byproduct and year |
| `sw2_disaggregation_proxies.xlsx` | Spatial disaggregation proxies by industry used to allocate national demand to the state level |
| `sw3_validation.xlsx` | External benchmark data used to validate demand estimates |

### `data/outputs/`
| File | Description |
|------|-------------|
| `results.csv` | Final dataset of annual state-level demand and national prices for 16 brine byproducts (2021–2025) |

### `figures/`
Key visualizations.

### `submodules/gw-avail-and-comp/`
A submodule with relevant data processing functions used to execute demand calculations and visualization. Note that the dependencies listed in `environment.yml` in this submodule are sufficient for this repository as well.
