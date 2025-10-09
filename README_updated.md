# 🌧️ Seattle vs. Portland Weather Analysis

> An analysis comparing rainfall frequency and intensity between Seattle, WA and Portland, OR using NOAA precipitation data from 2018–2022.

## Project Overview

This project investigates the popular belief that it rains more in Seattle than in Portland. Using data science methods and daily precipitation data from NOAA, the analysis determines whether the difference lies in total rainfall, frequency, or intensity.

- **Objective:** Determine whether Seattle experiences more rain than Portland, and whether the difference is in the number of rainy days or total precipitation.  
- **Domain:** Climate / Environmental Data Analysis  
- **Key Techniques:** Data cleaning and wrangling, exploratory visualization, statistical hypothesis testing (t-test and z-test)

## Project Structure

```
├── data/                 # Raw and cleaned precipitation data (NOAA)
├── code/                 # Main analysis notebook (weather_project.ipynb)
├── reports/              # Communication assignment and figures
└── README.md             # Project documentation
```

## Data

- **Source:** [NOAA Climate Data Online (NCEI)](https://www.ncei.noaa.gov/cdo-web/)  
- **Description:**  
  Daily precipitation (in inches) for Seattle, WA and Portland, OR from January 1, 2018 to December 31, 2022.  
  Columns include `date`, `precipitation`, and `city`.  
- **License:** Public domain (U.S. Government data)

## Analysis

The notebook `code/weather_project.ipynb` performs the following steps:

1. **Data Cleaning:** Remove duplicates, ensure consistent data types, and combine both cities into one tidy dataset.  
2. **Exploration:** Generate visualizations comparing monthly rainfall, rainy-day proportions, and rainfall distributions.  
3. **Statistical Testing:**  
   - **t-test** compares mean daily precipitation by month.  
   - **z-test** compares the proportion of rainy days between cities.  
4. **Interpretation:** Summarize which months show significant differences.

## Results

- Both cities receive **about the same total annual rainfall** (~40 inches/year).  
- Seattle experiences **rain more frequently**, with smaller daily amounts (“drizzle effect”).  
- Portland’s rainfall occurs on **fewer days** but tends to be **heavier** when it rains.  
- Statistical results confirm significant differences in **rainy-day frequency** (February, July, August, and October) but not in overall volume.

## Authors

- **Bruna Macedo Porto** — [@brunamportoDS](https://github.com/brunamportoDS)

## License

This project uses NOAA public-domain climate data. All analysis code is provided under the MIT License.

## Acknowledgements

- Seattle University — Foundations of Data Science (DATA 5100)  
- NOAA National Centers for Environmental Information (NCEI)  
- Python libraries: `pandas`, `matplotlib`, `seaborn`, `scipy`, `statsmodels`
