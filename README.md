# Airport and Weather Data Analysis

This project analyzes U.S. airport geography and weather patterns using Python and pandas. The focus is on identifying:
1. The northernmost airport in the United States.
2. The easternmost airport in the United States.
3. The New York area airport (JFK, LGA, EWR) with the windiest weather on February 12, 2013.

## Project Overview

The analysis was conducted using the `nycflights13` dataset, which includes details on U.S. airports and weather data from 2013. This project demonstrates skills in data cleaning, filtering, and analysis using Python's `pandas` library. Key insights were drawn from the geographical locations of airports and the wind conditions in New York on the specified date.

## Datasets

The following datasets were used:
- **airports.csv**: Contains detailed information on U.S. airports, including their geographic coordinates.
- **weather.csv**: Contains weather data for 2013, including wind speeds at various airports.

These datasets were sourced from the [nycflights13 dataset](https://github.com/tidyverse/nycflights13/tree/main/data-raw).

## Analysis Steps

1. **Loading the Data**:
   The datasets were loaded using the `pandas` library, and the relevant columns (e.g., latitude, longitude, wind speed) were extracted for analysis.

2. **Finding the Northernmost and Easternmost Airports**:
   The northernmost airport was identified based on the highest latitude, and the easternmost airport was found using the highest longitude.

3. **Wind Speed Analysis**:
   The weather data was filtered to focus on February 12, 2013, and wind speeds at JFK, LGA, and EWR were compared to identify the windiest airport.

4. **Outlier Handling**:
   The wind speed data for Newark (EWR) showed an unrealistic outlier, which was treated as a data entry error and excluded from the final analysis.

## Results

- **Northernmost Airport**: Dillant Hopkins Airport (FAA Code: EEN) at latitude 72.27.
- **Easternmost Airport**: Eareckson As (FAA Code: SYA) at longitude 174.11.
- **Windiest New York Airport on February 12, 2013**: LaGuardia Airport (LGA) with a wind speed of 23.02 m/s.

## Technologies Used

- **Python**: For data analysis.
- **pandas**: For loading, filtering, and analyzing the data.
- **Jupyter Notebook**: For interactive data exploration and analysis.

## Running the Code

To replicate the analysis:
1. Clone this repository.
2. Ensure you have Python installed along with the necessary libraries (`pandas` and `jupyter`).
3. Open the `AirportandWeatherAnalysis.ipynb` file in Jupyter Notebook and run the code cells sequentially.

You can install the required libraries by running:
```bash
pip install pandas jupyter
