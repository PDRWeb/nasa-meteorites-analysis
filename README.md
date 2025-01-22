# NASA Meteorite Project

## Table of Contents
- [Background and Overview](#background-and-overview)
- [Data Structure Overview](#data-structure-overview)
- [Executive Summary](#executive-summary)
- [Insights Deep Dive](#insights-deep-dive)
- [Recommendations](#recommendations)
- [Clarifying Questions, Assumptions, and Caveats](#clarifying-questions-assumptions-and-caveats)
- [Project Organization](#project-organization)

## Background and Overview
The purpose of this data analysis project is to analyze meteorite landings data provided by NASA. The goal is to identify patterns and insights that can help in understanding the distribution, composition, and frequency of meteorite landings on Earth. This analysis will answer key questions such as:
- What are the most common types of meteorites?
- Where are meteorites most commonly found?
- What is the average size and weight of meteorites?

## Data Structure Overview
The dataset consists of several columns, including:
- `name`: The name of the meteorite.
- `id`: A unique identifier for the meteorite.
- `recclass`: The classification of the meteorite.
- `mass (g)`: The mass of the meteorite in grams.
- `fall`: Whether the meteorite fell or was found.
- `year`: The year the meteorite was observed.
- `reclat`: The latitude where the meteorite was found.
- `reclong`: The longitude where the meteorite was found.
- `GeoLocation`: The geographical location (latitude, longitude).

A diagram of the data structure can viewed [here](https://dbdiagram.io/d/Meteorite-Landings-6790250137f5d6cbeb7e08e9).

## Executive Summary
This analysis reveals several critical insights:
1. **Common Meteorite Types**: The most common meteorite classifications are `L5`, `H5`, and `L6`.
2. **Geographical Distribution**: Meteorites are most commonly found in Antarctica, North America, and Africa.
3. **Meteorite Mass**: The average mass of meteorites varies significantly, with some weighing less than a gram and others over a ton.
4. **Temporal Patterns**: There is a noticeable increase in meteorite findings in recent years, likely due to improved detection methods.
5. **Fall vs. Found**: A majority of meteorites are found rather than observed falling.

Here is interactive [Tableau Public Dashboard](https://public.tableau.com/app/profile/paul.rodriguez7799/viz/nasa_FtoT/Dashboard) for deeper insights.

## Insights Deep Dive
### Common Meteorite Types
The dataset shows that `L5`, `H5`, and `L6` are the most frequently occurring meteorite classifications. These types are stony meteorites, which are the most common type found on Earth.

### Geographical Distribution
Meteorites are predominantly found in Antarctica due to the continent's ice sheets, which make meteorites easier to spot. North America and Africa also have high numbers of meteorite findings, likely due to extensive search efforts and favorable conditions for preservation.

### Meteorite Mass
The mass of meteorites ranges from a few grams to several tons. The largest meteorite in the dataset weighs over 60 tons. The distribution of meteorite mass is highly skewed, with most meteorites weighing less than a kilogram.

### Temporal Patterns
There has been a significant increase in the number of meteorites found in the last few decades. This trend is attributed to advancements in technology and increased interest in meteorite hunting.

### Fall vs. Found
The data indicates that most meteorites are found long after they have fallen, rather than being observed during their fall. This suggests that many meteorites go unnoticed when they initially land.

## Recommendations
Based on the insights gained from this analysis, the following recommendations are made:
1. **Increase Search Efforts in Underexplored Areas**: Focus on regions with fewer meteorite findings to potentially discover new meteorite types.
2. **Enhance Detection Methods**: Invest in technology to improve the detection and tracking of meteorites as they enter the Earth's atmosphere.
3. **Public Awareness Campaigns**: Educate the public on how to identify and report meteorite findings to increase the number of documented meteorites.

## Clarifying Questions, Assumptions, and Caveats
### Questions for Stakeholders Prior to Project Advancement
- Are there any specific meteorite classifications of interest?
- Should the analysis focus on a particular geographical region?
- Are there any known biases in the data collection process?

### Assumptions and Caveats
- **Assumptions**: It is assumed that the dataset provided by NASA is accurate and complete. The analysis also assumes that the geographical coordinates are correctly recorded.
- **Caveats**: The dataset may have biases due to uneven search efforts across different regions. Additionally, some meteorites may have been misclassified or not reported.

--------

## Project Organization

```
├── LICENSE            <- Open-source license
├── README.md          <- The top-level README for developers using this project
├── creative           <- Images/Video for the dashboard
|   
├── data
│   ├── external       <- Data from third party sources
│   ├── interim        <- Intermediate data that has been transformed
│   ├── processed      <- The final, canonical data sets for modeling
│   └── raw            <- The original, immutable data dump
│
├── models             <- Trained and serialized models, model predictions, or model summaries
│
├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
│                         the creator's initials, and a short `-` delimited description, e.g.
│                         `1.0-jqp-initial-data-exploration`
│
├── references         <- Data dictionaries, manuals, and all other explanatory materials
│
├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
│   └── figures        <- Generated graphics and figures to be used in reporting
│
├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
│                         generated with `pip freeze > requirements.txt`
│
├── src                         <- Source code for this project
    │
    ├── __init__.py             <- Makes src a Python module
    │
    ├── config.py               <- Store useful variables and configuration
    │
    ├── dataset.py              <- Scripts to download or generate data
    │
    ├── features.py             <- Code to create features for modeling
    │
    │    
    ├── modeling                
    │   ├── __init__.py 
    │   ├── predict.py          <- Code to run model inference with trained models          
    │   └── train.py            <- Code to train models
    │
    ├── plots.py                <- Code to create visualizations 
    │
    └── services                <- Service classes to connect with external platforms, tools, or APIs
        └── __init__.py 
└── workbook            <- Tableau packaged workbook file location
```

--------
