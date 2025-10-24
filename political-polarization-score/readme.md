# Political polarization score - Data package

This data package contains the data that powers the chart ["Political polarization score"](https://ourworldindata.org/grapher/political-polarization-score?v=1&csvType=full&useColumnShortNames=false) on the Our World in Data website. It was downloaded on October 12, 2025.

### Active Filters

A filtered subset of the full data was downloaded. The following filters were applied:

## CSV Structure

The high level structure of the CSV file is that each row is an observation for an entity (usually a country or region) and a timepoint (usually a year).

The first two columns in the CSV file are "Entity" and "Code". "Entity" is the name of the entity (e.g. "United States"). "Code" is the OWID internal entity code that we use if the entity is a country or region. For normal countries, this is the same as the [iso alpha-3](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-3) code of the entity (e.g. "USA") - for non-standard countries like historical countries these are custom codes.

The third column is either "Year" or "Day". If the data is annual, this is "Year" and contains only the year as an integer. If the column is "Day", the column contains a date string in the form "YYYY-MM-DD".

The final column is the data column, which is the time series that powers the chart. If the CSV data is downloaded using the "full data" option, then the column corresponds to the time series below. If the CSV data is downloaded using the "only selected data visible in the chart" option then the data column is transformed depending on the chart type and thus the association with the time series might not be as straightforward.

## Metadata.json structure

The .metadata.json file contains metadata about the data package. The "charts" key contains information to recreate the chart, like the title, subtitle etc.. The "columns" key contains information about each of the columns in the csv, like the unit, timespan covered, citation for the data etc..

## About the data

Our World in Data is almost never the original producer of the data - almost all of the data we use has been compiled by others. If you want to re-use data, it is your responsibility to ensure that you adhere to the sources' license and to credit them correctly. Please note that a single time series may have more than one source - e.g. when we stich together data from different time periods by different producers or when we calculate per capita metrics using population data from a second source.

## Detailed information about the data


## Political polarization score – V-Dem
Central estimate of the extent to which society is divided into hostile political camps, where political differences undermine social relationships and discourage interaction across ideological lines.
Last updated: March 17, 2025  
Next update: March 2026  
Date range: 1900–2024  


### How to cite this data

#### In-line citation
If you have limited space (e.g. in data visualizations), you can use this abbreviated in-line citation:  
V-Dem (2025) – processed by Our World in Data

#### Full citation
V-Dem (2025) – processed by Our World in Data. “Political polarization score – V-Dem” [dataset]. V-Dem, “Democracy report v15” [original data].
Source: V-Dem (2025) – processed by Our World In Data

### What you should know about this data
* We provide two kinds of regional averages: **country averages** and **population-weighted averages**. Country averages weigh each country equally and give a sense of how the typical country is doing. Population-weighted averages weigh countries with larger populations more and therefore better reflect the average person's experience.

### How is this data described by its producer - V-Dem (2025)?
Question: Is society polarized into antagonistic, political camps?

Clarification: Here we refer to the extent to which political differences affect social relationships beyond political discussions. Societies are highly polarized if supporters of opposing political camps are reluctant to engage in friendly interactions, for example, in family functions, civic associations, their free time activities and workplaces

Responses:
- 0: Not at all. Supporters of opposing political camps generally interact in a friendly manner.
- 1: Mainly not. Supporters of opposing political camps are more likely to interact in a friendly than a hostile manner.
- 2: Somewhat. Supporters of opposing political camps are equally likely to interact in a friendly or hostile manner.
- 3: Yes, to noticeable extent. Supporters of opposing political camps are more likely to interact in a hostile than friendly manner.
- 4: Yes, to a large extent. Supporters of opposing political camps generally interact in a hostile manner.

Scale: Ordinal, converted to interval by the measurement model.

Indicator nanme: `v2cacamps`

### Source

#### V-Dem – Democracy report
Retrieved on: 2025-03-17  
Retrieved from: https://v-dem.net/data/the-v-dem-dataset/  

#### Notes on our processing step for this indicator
### Region aggregates
The default regional aggregates (including values for the World) have been estimated by averaging the country values. These are only estimated when data for most countries and populations is available (i.e. 70% for most continents). We have used the list of countries in 1900 as a reference.

In addition, regional aggregates with names like "Region (population-weighted)" (including values for World) have been estimated by averaging the country values weighted by population. The population values are from the UN WPP 2024 revision dataset. These are only estimated when 70% of people in region have data for the given year.

### Data imputation
We expand the years covered by V-Dem further: To expand the time coverage of today's countries and include more of the period when they were still non-sovereign territories, we identified the historical entity they were a part of and used that regime's data whenever available

For example, V-Dem only provides regime data since Bangladesh's independence in 1971. There is, however, regime data for Pakistan and the colony of India, both of which the current territory of Bangladesh was a part. We, therefore, use the regime data of Pakistan for Bangladesh from 1947 to 1970, and the regime data of India from 1789 to 1946. We did so for all countries with a past or current population of more than one million.

For more details on the imputation methodology and which countries are affected, refer to [this file](https://github.com/owid/etl/blob/master/etl/steps/data/garden/democracy/2025-03-17/vdem/vdem.countries_impute.yml).


    