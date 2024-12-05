# Tornado Trend Analysis Case Study

**A DS 4002 Case Study by Zaid Fada**

**Date**: December 9th 2024

## Project Overview

This repository contains the code, data, and documentation for the Tornado Trend Analysis project. In this case study, we analyze tornado trends in the U.S. from 1999 to 2023 to develop time-series prediction models using ARIMA and SARIMA. The goal is to predict tornado-related metrics such as property damage, fatalities, and frequency with the aim of minimizing Mean Absolute Error (MAE). This analysis contributes to a better understanding of long-term trends in tornado activity and aims to improve disaster response strategies.

The case study is targeted at a second-year UVA student, providing an engaging way to apply data science techniques to a real-world problem involving disaster preparedness.

## Hook and Rubric Documents

The **hook document** outlining the case study is titled _CS3-Hook.pdf_. This document provides an overview of the case study and aims to get students interested in the analysis. The **rubric** (_C3-Rubric.pdf_) outlines the formatting, submission requirements, and final deliverables for this assignment. Both documents should be continuously referenced throughout the completion of the case study to guarantee success on the assignment.

## Repository Structure

```bash
.
├── README.md                # Project overview and instructions for reproducing results
├── LICENSE.md               # License information (MIT)
├── requirements.txt         # Python packages needed for the project
├── CS3-Hook.pdf         # Hook document for the case study
├── CS3-Rubric.pdf       # Rubric document for the case study
├── MATERIALS/ARTICLES/
│   ├── TwistersAndTrends-AnAnalysisOfUSTornadoActivityAndClimateChange.pdf        
│   ├── ArimaAndSarima.pdf
├── MATERIALS/SCRIPTS/
│   ├── 1-data.ipynb         # Data preparation script to combine data over the years
│   ├── 2-exploratory.ipynb  # Preliminary data discovery and exploratory analysis
│   ├── 3-analysis.ipynb     # Detailed step-by-step analysis and model implementation
│   └── 4-stats.ipynb        # Statistical analysis and interpretation of results
├── MATERIALS/DATA/
│   └── Data.md              # Steps to download the dataset and data dictionary
├── MATERIALS/OUTPUT/
│   └── plots/               # Figures generated during data

```

## Software and Platform

- **Programming Language**: Python
- **Packages Required**:

  - `pandas`
  - `numpy`
  - `scikit-learn`
  - `scipy`
  - `matplotlib`
  - `statsmodels`

- **Platform**: Windows, macOS, or Linux

## Data

The dataset for this project is sourced from the "NCDC Storm Events Database" and includes comprehensive tornado event data across the U.S. from 1999 to 2023. It contains information such as the date, location, injuries, fatalities, and property damage for each tornado event.

## Instructions for Reproducing Results

1. Clone this repository:

   ```bash
   git clone [repository link]
   cd [repository directory]
   ```

2. Install the required Python packages: Ensure that Python 3.x is installed. Then, install the necessary packages by running:
   ```bash
   pip install -r requirements.txt
   ```
3. Download and prepare the data:

   - Go to the `1-data.ipynb` to see HOW we created the combined-df file, however, I decided not to include every individual csv as it would have been too much data
   - The dataset (combined_df) is in the `DATA/` folder

4. Run the exploratory plots:

   - Go to `/SCRIPTS/2-exploratory.ipynb`, follow the comments in the cells and run each cell to see our exploratory-plots, or go to outputs to see them directly!

5. Run the analysis:

   - Go to `/SCRIPTS/3-analysis.ipynb`, follow the comments in the cells and run each cell to perform our analysis!

6. Run the stats:

   - Go to `/SCRIPTS/5-stats.ipynb`, follow the comments in the cells and run each cell to see where we got our takeaways from!

7. Review the results:
   - The model’s accuracy, precision, recall, and other performance metrics will be saved in the [results.md](OUTPUTS/results.md) file
   - Visualizations will be saved in the `OUTPUTS/plots/` directory.

# Tornado Analysis Results

The analysis involved comparing tornado characteristics over the years, focusing on:

- Proportion of Severe Tornadoes (F3 and Above)
- Proportion of Injury-Causing Tornadoes
- Tornado Counts by F-Scale
- Trends in Tornado Frequency

## Summary

- Increasing Severity: The proportion of tornadoes classified as F3 and above has increased significantly over the years.
- Decreasing Injuries: The proportion of injury-causing tornadoes has decreased, possibly due to improved early warning systems and preparedness.
- Shifts in Tornado Frequency by Scale: There has been a notable shift in the frequency of tornado intensities, indicating a possible change in climate patterns affecting tornado activity.

These insights could prove valuable in allocating resources for disaster management and developing proactive policies to protect vulnerable regions.

# References

[1] National Centers for Environmental Information, “Storm Events Database CSV Files.” [Online]. Available: https://www.ncei.noaa.gov/pub/data/swdi/stormevents/csvfiles/. [Accessed: Oct. 31, 2024].

[2] Yennhi95zz, “A Guide to Time Series Models in Machine Learning: Usage, Pros, and Cons,” Medium, Jul. 28, 2019. [Online]. Available: https://medium.com/@yennhi95zz/a-guide-to-time-series-models-in-machine-learning-usage-pros-and-cons-ac590a75e8b3. [Accessed: Oct. 31, 2024].

[3] S. Berdiales, _Forecasting Models: ARIMA_, bookdown.org, 2020. [Online]. Available: https://bookdown.org/sergioberdiales/tfm-kschool_gijon_air_pollution/forecasting-models-arima.html. [Accessed: Oct. 31, 2024].
