
# Weather Data (Central African Region)

## Description

This dataset contains processed meteorological time-series data derived from gridded weather observations over the Congo region. It is designed to support research in short-term rainfall prediction using machine learning and deep learning techniques.

The dataset is constructed from large-scale raw gridded meteorological data collected over approximately ten years. The raw data consists of millions of observations distributed across multiple spatial grid points, each defined by latitude, longitude, and elevation. A multi-stage preprocessing pipeline was applied, including data extraction, cleaning, temporal alignment, and feature engineering. The resulting dataset is structured and suitable for time-series modeling.

This dataset does **not include a predefined target variable**, allowing users to define their own prediction tasks such as rainfall occurrence classification or rainfall intensity estimation.

---

## Geographic Coverage

- Region: **Central Africa**
- Data type: **Gridded spatial observations**
- Each observation corresponds to:
  - Latitude
  - Longitude
  - Elevation

---

## Data Source

- Source: **Open-Meteo API**
- Data type: **Gridded meteorological data**
- Temporal resolution: **Hourly**
- Time coverage: **~10 years**

---

## Dataset Characteristics

- Type: **Multivariate meteorological time-series data**
- Spatial structure: **Grid-based (multiple locations per timestamp)**
- Processed dataset size: ~87,000 samples
- Raw dataset size: Millions of observations

---

## Features

The raw dataset includes both meteorological variables and structured metadata.
The raw dataset (millions of rows) was transformed into a compact dataset (~87,000 samples) optimized for modeling with features such as:

### Meteorological Variables

- Temperature
- Humidity
- Wind speed
- Wind direction
- Atmospheric pressure
- Precipitation

### Engineered Features

- Temporal features (e.g., hour, day, seasonal indicators)
- Physically informed features (e.g., upstream indicators derived from neighboring grid cells)

---

## Data Processing

The dataset was generated through a multi-stage preprocessing pipeline:

- Extraction of meteorological variables from gridded data
- Handling missing and inconsistent observations
- Spatial-to-temporal transformation of grid data
- Temporal alignment at hourly resolution
- Feature engineering, including upstream atmospheric indicators
- Construction of structured time-series data suitable for machine learning

---