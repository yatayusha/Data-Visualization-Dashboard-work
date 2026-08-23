# Eurovision Data Analysis

https://colab.research.google.com/drive/1b0lYRvzWj9DuDt68t4-Fp-l2WHd7Tf2i?usp=sharing

## Overview

An exploratory data analysis project examining musical characteristics and historical performance patterns of Eurovision entries.

The project focuses on transforming raw song data into structured numerical features and using statistical visualisation to explore relationships between music characteristics, genres, participant demographics, and country performance.

## Questions Explored

The analysis addresses questions such as:

* Which musical characteristics are correlated with each other?
* Is there a relationship between a song's happiness and energy?
* Which genres are most represented in the dataset?
* Which countries have achieved the highest number of Eurovision wins?
* How has participant gender distribution changed over time?
* Which countries demonstrate the most consistent final rankings?
* Which countries most frequently reach the final and place in the top three?

## Data Preparation

The dataset contained musical and competition-related attributes for Eurovision entries.

The preprocessing pipeline included:

* Handling missing values and invalid placeholders in numerical columns
* Cleaning `loudness` values by removing measurement units
* Converting musical features to numerical `float` data types
* Preparing a clean dataset for exploratory analysis and visualisation

Key musical features included:

`BPM` · `energy` · `danceability` · `happiness` · `acousticness` · `instrumentalness` · `liveness` · `speechiness` · `loudness`

## Analysis

### Feature Correlation

A correlation matrix was used to examine relationships between musical characteristics.

The analysis highlighted how features such as energy, happiness, and other audio characteristics move together and provided a foundation for further exploration.

### Happiness and Energy

A scatter plot was used to explore the relationship between happiness and energy.

Average values were added as reference lines to improve interpretation of the distribution and identify observations across different quadrants.

The results suggest a positive association: tracks with higher happiness scores tend to also exhibit higher energy levels.

### Genre Distribution

The distribution of songs across genres was analysed using sorted bar charts.

Pop was the most represented genre in the dataset.

### Danceability Across Genres

Density plots and histograms were used to compare danceability distributions across genres.

The analysis showed that average danceability generally reflected genre characteristics, while categories with limited observations produced less reliable estimates.

### Country Performance

Several visualisations were used to analyse Eurovision performance across countries:

* Number of victories
* Years of victories
* Distribution of final rankings
* Consistency and variability of results
* Number of appearances in the final
* Frequency of top-three finishes

Countries with lower median final positions demonstrated stronger overall performance, while the spread of rankings provided insight into the consistency of results.

### Geographic Analysis

A choropleth map was used to visualise how frequently countries represented in the dataset reached the Eurovision final.

### Top Three Performance

A treemap was used to compare countries with multiple top-three finishes.

Filtering out isolated successes made it possible to focus on countries demonstrating consistently strong performance.

## Visualisation Techniques

The project uses multiple visualisation libraries to compare static and interactive approaches:

* Seaborn
* Matplotlib
* Plotly
* Altair
* Folium
* GeoPandas

Visualisations include:

* Correlation heatmaps
* Scatter plots
* Bar charts
* Density plots
* Histograms
* Box plots
* Pie charts
* Choropleth maps
* Treemaps

## Key Takeaways

* Musical features show meaningful relationships that can be explored through correlation analysis.
* Happiness and energy demonstrate a positive association.
* Pop is the most represented genre in the dataset.
* Country performance can be analysed not only through wins, but also through ranking consistency and distribution.
* Geographic and hierarchical visualisations provide complementary views of Eurovision performance.

## Tech Stack

**Python** · **Pandas** · **NumPy** · **Matplotlib** · **Seaborn** · **Plotly** · **Altair** · **Folium** · **GeoPandas**

## Repository Structure

```text
eurovision-data-analysis/
│
├── notebooks/
│   └── eurovision_data_analysis.ipynb
│
├── data/
│   └── song_data.csv
│
├── images/
│   ├── correlation_heatmap.png
│   ├── happiness_vs_energy.png
│   ├── genre_distribution.png
│   ├── country_performance.png
│   └── eurovision_map.png
│
├── requirements.txt
└── README.md
```

## Project Focus

This project demonstrates an end-to-end exploratory data analysis workflow:

**Raw Data → Cleaning → Feature Preparation → Exploratory Analysis → Visualisation → Insight Generation**
