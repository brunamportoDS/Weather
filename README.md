Seattle vs. Portland Weather Analysis

An analysis comparing rainfall frequency and intensity between Seattle, WA and Portland, OR using NOAA precipitation data from 2018–2022.

Project Overview

This project investigates wheather it rains more in Seattle than in Portland. Using data science methods and daily precipitation data from NOAA, the analysis determines whether the difference lies in total rainfall, frequency, or intensity.

Objective: Determine whether Seattle experiences more rain than Portland, and whether the difference is in the number of rainy days or total precipitation.

Domain: Climate / Environmental Data Analysis

Key Techniques: Data cleaning and wrangling, exploratory visualization, statistical hypothesis testing (t-test and z-test)

Weather/
├── code/
│   └── weather_project.ipynb
├── reports/
│   ├── Weather_communicate_the_results.docx
│   └── figures/ (optional, if you add PNGs or charts)
├── data/
│   └── clean_weather_data.csv (optional)
└── README.md


Data
Seattle data - https://raw.githubusercontent.com/brian-fischer/DATA-5100/refs/heads/main/weather/seattle_rain.csv
Portland data - https://raw.githubusercontent.com/brian-fischer/DATA-5100/refs/heads/main/weather/seattle_rain.csv

Source: NOAA Climate Data Online (NCEI)

Description:
Daily precipitation (in inches) for Seattle, WA and Portland, OR from January 1, 2018 to December 31, 2022.
Columns include date, precipitation, and city.

License: Public domain (U.S. Government data)

Analysis

The notebook code/weather_project.ipynb performs the following steps:

Data Cleaning: keep only the relevant columns, convert date columns to datetime format,add a 'city' label, and combine both datasets. Column with months extracted from dates was created to facilitate exploration.

Exploration: Generate visualizations comparing monthly rainfall, rainy-day proportions, and rainfall distributions.

Statistical Testing:

t-test compares mean daily precipitation by month.

z-test compares the proportion of rainy days between cities.

Interpretation: Summarize which months show significant differences.

Results
Seattle and Portland receive about the same amount of rain each year, but Seattle’s rainfall occurs more often and in smaller amounts. The data support Seattle’s reputation for frequent drizzle, but not necessarily harder or longer. Portland, by contrast, experiences similar rainfall totals condensed into fewer, heavier events.

Authors

Bruna Macedo Porto — @brunamportoDS

License

This project uses NOAA public-domain climate data. All analysis code is provided under the MIT License.

Acknowledgements

Seattle University — Foundations of Data Science (DATA 5100)

NOAA National Centers for Environmental Information (NCEI)

Python libraries: pandas, matplotlib, seaborn, scipy, statsmodels
