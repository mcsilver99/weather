# Seattle versus Boston Weather Project

> This project aims to compare precipitation in Seattle and Boston to determine where if it rains more in one city than the other. 

---

## Project Overview

This project aims to answer the question of whether it rains more in Seattle than in Boston. The data used is is from the National Oceanic and Astmostpheric Agency. It contains precipitation data for cities, Seattle and Boston over a five year period. 

- **Objective:** Ascertain if it rains more in Seattle or Boston. 
- **Domain:** Weather
- **Key Techniques:** Descriptive statistics, graphs, t-test, z-test

---

## Project Structure

```
├── data/                 # Raw and processed data
├── code/                 # Jupyter notebooks and Python scripts
├── reports/              # Generated reports and visualizations
├── requirements.txt      # Dependencies
└── README.md             # Project documentation
```

---

## Data

- **Source:** https://www.ncei.noaa.gov/cdo-web/
- **Description:** The Seattle and Boston data sets were downloaded from the National Oceanic and Atmospheric Administration wesbite in CSV format. The Seattle data set had  1,658 observations and 10 columns, while the Boston data had 1,826 observations and 5 columns. Both data sets contained data from only 1 station and contained the columns needed to achieve the objective: Date and Precipitation. 
- **License:** N/A. This data is available to the public.

---

## Analysis

The tidy data set (clean_seattle_boston_weather.csv) has 1826 rows for each city for date range between January 1, 2019 and December 31, 2022. It has 3 columns: Date, City, and Precipitation (inches). The data used to answer the question of whether it rains more in Seattle or Boston, was collected from a single station near the major airport of each city, respectively. We wanted all precipitation data from all days in the date range January 1, 2018, to December 31, 2022. The Boston data had precipitation values for all days in the date range, but Seattle had 90 days where data was not recorded. We replaced those values with the average rainfall for that day across the remaining years. By the end of the data processing phase, we had a clean, tidy data set that had precipitation values in inches for every day in the desired date range.

In the analysis phase, precipitation patterns in Seattle and Boston were visualized by summarizing daily and monthly averages and comparing rainfall distributions and frequency of rainy days. In the modeling phase, two-sided t-tests and z-tests were used to assess whether differences in average rainfall and the proportion of rainy days between the two cities were statistically significant.

To reproduce the results, run the code in order: Import Libraries, Load Data, Explore the Data, Clean the Data, and Analyze. 


---

## Results

The results of the study over the five-year period show Boston has higher mean daily precipitation than Seattle, but it rains more frequently in Seattle. However, in July and August Boston has a higher mean nonthly precipitation, and higher proportion of days with any rain than Seattle. See a more in depth analysis with supporting graphs in the Results document located in the reports folder. 

---

## Authors

- Maya Silver- [@mcsilver99](https://github.com/mcsilver99)

---

## License

- Everyone in the MSDS program at Seattle University may access and use the project materials in this repository. Anyone else must request the author's permission. 

---

## Acknowledgements

- Jupyter Lab, scipy (for statistical tests)
- 
