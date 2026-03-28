# NOAA Lightning Strike Analysis (EDA Structuring)

---

# For This Part of the Project

## Background

The National Oceanic and Atmospheric Administration (NOAA) collects lightning strike data using satellite-based systems capable of detecting both cloud-to-ground and in-cloud activity. These datasets include detailed records of strike frequency, location, and timing.

In this project, multi-year NOAA data is structured and integrated to support consistent analysis. Feature engineering is used to extract temporal components such as weekday, week, month, and year, enabling comparisons across time. This allows for the analysis of spatial concentration, frequency of lightning by location, and variation in strike patterns across days and seasons.

The data sourced from NOAA’s Geostationary Lightning Mapper (GLM), is provided as a structured dataset for analysis and is broken up into two parts for this project. I was able to provide one dataset on this repository, however, becuase of Github's file size limit (25mb) I could not upload the second. Methods utilizing zip and parquet could not compress the file. In its raw form, the data can be found publicly available on the NOAA website via 'Archives'.

---

## Project Goal

The goal of this phase is to structure and prepare multi-year NOAA lightning strike data for exploratory analysis.

This involves organizing the structured dataset and establishing a baseline understanding of how lightning activity varies across:

- Geographic location  
- Time (weekday patterns)  
- Seasonal trends (monthly and yearly distribution)  

The objective is to create a clean and structured dataset that supports identifying patterns and relationships in lightning activity across multiple scales.

---

## Tools & Technologies

- **Environment:** Jupyter Notebook  
- **Language:** Python  
- **Libraries:** NumPy, Pandas, Seaborn, Matplotlib, Datetime  
- **Techniques:** Data structuring, datetime conversion, groupby(), aggregation (agg), value_counts(), merge()  

---

### Insights  

**Patterns observed in lightning activity:**

- **Geographic concentration**  
  - Certain locations consistently experience higher strike frequency  
  - High-activity regions tend to appear in close proximity  

- **Temporal consistency (weekly)**  
  - Weekday distributions remain relatively stable  
  - Slight weekend decreases do not significantly impact overall patterns  

- **Seasonal variation (multi-year)**  
  - Lightning activity is not evenly distributed throughout the year  
  - Activity increases over time and peaks during late summer months  

---

## Project Overview

### Key Takeaways  

Lightning activity is not evenly distributed across either geographically or temporally.

A relatively small number of locations appear repeatedly with higher strike frequency, indicating geographic clustering rather than random distribution. The most extreme events also tend to occur within these concentrated regions.

Across weekdays, activity remains fairly stable. While there is a slight decrease on weekends, the overall distribution does not meaningfully shift.

More noticeable variation appears across longer time periods. Lightning activity builds throughout the year and peaks during specific seasonal windows, with late summer showing the highest concentration of strikes.

### The "So What?"

The three year snapshot (2016-2018) provided by this dataset reveals consistent trends across seasonal lightning patterns suggesting that events are not so random and can be anticipated to some extent.

Geographic concentration further highlights areas where activity remains consistently higher setting a strong starting point for improved target monitoring and deeper analysis into other factors that may be driving this behavior.
