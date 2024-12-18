# Classification Model for Music Lyrics

**Case Study Owner**: Malek Thabet
**Date**: 09 December 2024

## Project Overview

This repository contains the code, data, and documentation to classify musical genres based solely on lyrical data using an Random Forest classification model. The goal is to achieve an accuracy of 60% or greater in genre classification using the “English Music Lyrics from Five Music Genres” dataset from Kaggle. The analysis will focus on feature extraction and model training to improve classification performance.

## Repository Structure

- **Hook.pdf**: Motivation for project
- **Rubric.pdf**: Outlining of deliverables and rubric
- **LICENSE.md**: License for the project (MIT License).
- **requirements.txt**: Python packages needed for the project
- **Materials/**: Contains the data as well as Python scripts for data processing, feature engineering, and model training

```bash
.
├── Hook.pdf                 # Deliverables and motivation for the case
├── Rubric.pdf               # How to measure success of the work
├── README.md                # Project overview and instructions
├── LICENSE.md               # License information (MIT)
├── requirements.txt         # Python packages needed for the project
├── Materials/
│   ├── exploratoryplots.ipynb  # Prelim data discobvery
│   └── analysis.ipynb       # Detailed step-by-step analysis performed
│   └── Data.md              # Steps to download dataset
```

## Software and Platform

- **Programming Language**: Python
- **Packages Required**:
  - `pandas`
  - `numpy`
  - `scikit-learn`
  - `seaborn`
  - `matplotlib`
  - `wordcloud`
- **Platform**: Windows, macOS, or Linux

## Data

The dataset used for this project is the "English Music Lyrics from Five Music Genres" dataset from Kaggle, which contains 500,000 song lyrics from five genres: country, metal, rock, pop, and rap.

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

   - Go to the `DATA.md` and follow the steps to download our data
   - Place the dataset in the `Materials/` folder

4. Run the analysis:

   - Go to `/Materials/ANALYSIS.ipynb`, follow the comments in the cells and run each cell to perform our analysis!

