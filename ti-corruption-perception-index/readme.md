# Corruption Perceptions Index - Data package

This data package contains the data that powers the chart ["Corruption Perceptions Index"](https://ourworldindata.org/grapher/ti-corruption-perception-index?v=1&csvType=full&useColumnShortNames=false) on the Our World in Data website.

## CSV Structure

The high level structure of the CSV file is that each row is an observation for an entity (usually a country or region) and a timepoint (usually a year).

The first two columns in the CSV file are "Entity" and "Code". "Entity" is the name of the entity (e.g. "United States"). "Code" is the OWID internal entity code that we use if the entity is a country or region. For normal countries, this is the same as the [iso alpha-3](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-3) code of the entity (e.g. "USA") - for non-standard countries like historical countries these are custom codes.

The third column is either "Year" or "Day". If the data is annual, this is "Year" and contains only the year as an integer. If the column is "Day", the column contains a date string in the form "YYYY-MM-DD".

The remaining columns are the data columns, each of which is a time series. If the CSV data is downloaded using the "full data" option, then each column corresponds to one time series below. If the CSV data is downloaded using the "only selected data visible in the chart" option then the data columns are transformed depending on the chart type and thus the association with the time series might not be as straightforward.

## Metadata.json structure

The .metadata.json file contains metadata about the data package. The "charts" key contains information to recreate the chart, like the title, subtitle etc.. The "columns" key contains information about each of the columns in the csv, like the unit, timespan covered, citation for the data etc..

## About the data

Our World in Data is almost never the original producer of the data - almost all of the data we use has been compiled by others. If you want to re-use data, it is your responsibility to ensure that you adhere to the sources' license and to credit them correctly. Please note that a single time series may have more than one source - e.g. when we stich together data from different time periods by different producers or when we calculate per capita metrics using population data from a second source.

### How we process data at Our World In Data
All data and visualizations on Our World in Data rely on data sourced from one or several original data providers. Preparing this original data involves several processing steps. Depending on the data, this can include standardizing country names and world region definitions, converting units, calculating derived indicators such as per capita measures, as well as adding or adapting metadata such as the name or the description given to an indicator.
[Read about our data pipeline](https://docs.owid.io/projects/etl/)

## Detailed information about each time series


## Corruption Perceptions Index (CPI)
A country’s score, from 0 (most corrupt) to 100 (least corrupt), that reflects the average of expert surveys on public sector corruption, including misuse of office and bribery.
Last updated: May 13, 2025  
Next update: May 2026  
Date range: 2012–2024  


### How to cite this data

#### In-line citation
If you have limited space (e.g. in data visualizations), you can use this abbreviated in-line citation:  
Transparency International (2024) – with minor processing by Our World in Data

#### Full citation
Transparency International (2024) – with minor processing by Our World in Data. “Corruption Perceptions Index (CPI)” [dataset]. Transparency International, “Corruption Perceptions Index” [original data].
Source: Transparency International (2024) – with minor processing by Our World In Data

### What you should know about this data
* The Corruption Perceptions Index (CPI) ranks countries and territories based on the perceived level of public sector corruption, as judged by experts and business leaders.
* Depending on the country, it combines data up to 13 independent sources, including expert assessments and business surveys from trusted institutions.
* Each source is converted to a scale from 0 to 100, where 0 means very corrupt and 100 means very clean.
* A country’s CPI score is the simple average of the available sources for that year.
* The method has stayed the same since 2012, so scores can be compared over time.
* The CPI includes a 90% confidence interval (margin of error) to reflect differences between sources and possible inconsistencies.
* The CPI does not measure corruption directly. It measures perceptions, because there are no fully objective national measures of corruption.

### How is this data described by its producer - Transparency International (2024)?
The Corruption Perceptions Index (CPI) aggregates information from several sources that capture how business professionals and country experts perceive corruption in the public sector.

To build the CPI, eligible data sources are first selected. A source qualifies only if it measures public‑sector corruption perceptions; relies on a sound, comparable scoring method; is produced by a credible institution; shows enough score variation to differentiate countries; covers a substantial number of nations; bases its ratings on the views of country experts or businesspeople; and is updated at least every two years. The current CPI draws on 13 data sets supplied by 12 separate institutions, each reflecting perceptions recorded during the preceding two years (the accompanying source‑description document details them).

Next, every source is converted to a 0–100 scale, where 0 represents the highest perceived corruption and 100 the lowest. This standardisation subtracts the source’s baseline‑year mean from each country’s raw score and divides the result by that source’s baseline‑year standard deviation. The standardised value is then rescaled by multiplying by the CPI’s 2012 standard deviation (20) and adding the CPI’s 2012 mean (45), ensuring scores remain comparable across years while fitting the CPI’s 0–100 range.

Finally, a country or territory enters the CPI only when at least three separate sources assess it. The country’s CPI figure is the arithmetic mean of all its available standardised scores, rounded to the nearest whole number.

### Source

#### Transparency International – Corruption Perceptions Index
Retrieved on: 2025-05-13  
Retrieved from: https://www.transparency.org/en/cpi/2024  


## World regions according to OWID
Regions defined by Our World in Data, which are used in OWID charts and maps.
Last updated: January 1, 2023  
Date range: 2023–2023  


### How to cite this data

#### In-line citation
If you have limited space (e.g. in data visualizations), you can use this abbreviated in-line citation:  
Our World in Data – processed by Our World in Data

#### Full citation
Our World in Data – processed by Our World in Data. “World regions according to OWID” [dataset]. Our World in Data, “Regions” [original data].
Source: Our World in Data

### Source

#### Our World in Data – Regions


    