# Los Angeles County Oil Wells
Geospatial Research Project by: Katie Greenler, Madalyn Bryant, Divine Mutoni, Myranda Arreola, Luis Garcia Chavez
## **Introduction & Spatial Scope**
_What is the relationship between the proximity to active and closed/protected oil wells and socio-economic indicators in Los Angeles? Specifically, does proximity to an active oil well correlate with lower property values, decreased income, and a higher concentration of people of color? Conversely, is proximity to a closed/protected oil well associated with higher property values, increased income, and predominantly white communities?_

![Oil field in Inglewood, CA](https://ca-times.brightspotcdn.com/dims4/default/e26c0e0/2147483647/strip/true/crop/600x377+0+0/resize/1200x754!/quality/75/?url=https%3A%2F%2Fcalifornia-times-brightspot.s3.amazonaws.com%2Fc7%2Fa3%2F88276b303a8cc57a63d8ca957f48%2Fla-xpm-photo-2012-oct-10-la-me-fracking-baldwin-hills-20121010)

In the last two years, the city and county of Los Angeles voted to stop new oil extraction and phase out active oil extraction by 2043. At this moment in time there are 26 oil and gas fields with over 5,000 wells across Los Angeles county. These wells have significant polluting effects on the lives of the people who live right next to them as well as immediate and prolonged effects on the air, soil, and water throughout the county. 

The context of these wells, who extracts the profits, and who faces the most exposure are key questions for interventions and the urgency of where oil wells are shut down first and other reparative steps toward racial and economic justice in the city.

## **Datasets**
Many datasets are needed in order to properly investigate the current state of oil wells and their correlation with socioeconomic indicators. The primary dataset of focus for this project is the [LA County Oil Wells](https://geohub.lacity.org/datasets/29f5d6391d0749a7ac59aacd40bb0846/explore?location=33.800844%2C-118.295000%2C9.16) data from LA City GeoHub. The geojson provides the point locations for all of the wells in LA County as well as their status and which oil field they fall into. We plan to aggregate these point locations to the census tract level to allow for more easy comparison when needed but otherwise will display them as points. 

The base of our data, and later maps, will be composed of a mix of Census data and other indicators that help in answering and visualizing our proposed research question. At a high level we will use and reference data from [CalEnviroScreen](https://experience.arcgis.com/experience/ed5953d89038431dbf4f22ab9abfe40d/) as it is a reputable and comparable source used by many agencies and companies when looking at socio-economic and pollution burden within communities. This data provides a score for each census tract across California, so we will be clipping this data to the extent of LA County.

Our supplementary datasets are from the American Community Survey, specifically the 5-year estimates from 2022. We each took on data exploration for one the following themes: race & ethnicity, income, home values, education, and disability.

The [Race/Ethnicity data](https://www.socialexplorer.com/tables/ACS2022_5yr/R13563599) was retrieved from the Census Bureau and it features data on the total population, race, race by hispanic (collapsed version), and tenure - renter or homeowner by ethnicity. We anticipate using the race by hispanic variable to more closely align with the most commonly used categorization in Los Angeles, and conduct analysis on trends and patterns drawn along racial and/or ethnic lines. 

The [income census data](https://data.census.gov/table/ACSST5Y2022.S1901?t=Earnings%20(Individuals):Income%20(Households,%20Families,%20Individuals):Income%20and%20Earnings:Income%20and%20Poverty&g=050XX00US06037$1400000&y=2022&d=ACS%205-Year%20Estimates%20Subject%20Tables) was downloaded from the Census Bureau and was categorized into total household income, with columns representing various income brackets.

The [education census data](https://data.census.gov/table?t=Educational%20Attainment&g=050XX00US06037$1400000) was downloaded in csv format from the Census Bureau website. This file includes educational attainment, ranging from highschool to bachelor’s level, broken out by race and age.

The [data on disability](https://data.census.gov/table/ACSST5Y2022.S2701?q=health&g=050XX00US06037,06037$1400000&tid=ACSST1Y2022.S2701) was also downloaded from the Census Bureau with an emphasis on people with disabilities and the amount of people with health insurance by census tract.

The [home value data](https://data.census.gov/table/ACSDP5Y2022.DP04?q=value&t=HousingValueandPurchasePrice&g=050XX00US06037$1400000&y=2022) was downloaded from the Census Bureau with an emphasis on Home Values of owner-owned properties in Los Angeles Census Tracts. 

## **Scope of Intended Analysis**
**Deliverable**: A  story map of the current disparate impact of Los Angeles oil wells. We do not have oil well data for how this has happened in the past, but we may look at how some of the census factors have changed over time with knowledge of the political manifestations of the oil well deals. 

**Analysis**: The primary scope of this analysis is to highlight how the production of power and oil extraction is tied to power and vulnerability in the city. We will do so by examining levels of exposure to different resident groups, spatially mapping environmental injustices, and providing initial insight in a set or one specific policy recommendation/ intervention focusing on a handful of interventions  

- **Assess vulnerabilities and exposure along demographic indicators**: In particular, we seek to understand the relationship between different socioeconomic demographics indicators, and the risk exposure borne from proximity to power and oil extraction facilities. In a 2023 study on the racial and socioeconomic disparities in exposure to oil and gas development, the authors show that socioeconomically marginalized people had disproportionately high exposure to active wells throughout the study period (Gonzalez et al, 2023). Similarly, they show disproportionate risk borne by renters, non-voters, and low-income people based on the group’s risk ratio, a score that accounts for the group’s proportion in the exposed group as opposed to the overall population. We may consider replicating a similar formulation for Los Angeles county.

![Estimation of risk from oil wells by race, ethnicity, and income](https://agupubs.onlinelibrary.wiley.com/cms/asset/be2e3e5d-f6db-4d82-a5d3-4dc7a17e14f7/gh2410-fig-0003-m.png)

- **Mapping environmental injustices**: We can also see an opportunity to spatially illustrate how different oil wells bear negative environmental externalities, and how the burden varies across LA county. For instance, we can combine the geospatial oil well data, and Toxics Release Inventory Explorer’s data to show how exposure to toxins from oil wells differs and in what communities is such exposure highest. This exercise will leverage the spatial mapping tools introduced in class.

- **Developing a set of recommendations**: Our storyboard will conclude with a deep dive into possible policy recommendation(s) based on the findings. The group may choose to investigate for example funding going towards toxin reduction, and the mix of both community-level and business intervention mechanisms to ensure restorative environmental justice.

## **Goals and Insights**

Our goal is to comprehensively understand the dynamics between oil well statuses - both active and closed/protected - and socioeconomic indicators in Los Angeles. We aim to provide insights for addressing environmental injustices linked to the proximity of identified groups to oil wells.

### **Sources**
Bhavna Shamasunder and Jill E. Johnston, 2023: The Imperative of Equitable Protection: Structural Racism and Oil Drilling in Los Angeles. American Journal of Public Health 113, 1179_1181, https://doi.org/10.2105/AJPH.2023.307405

González, D. J. X., Morton, C. M., Hill, L. A. L., Michanowicz, D. R., Rossi, R. J., Shonkoff, S. B. C., et al. (2023). Temporal trends of racial and socioeconomic disparities in population exposures to upstream oil and gas development in California. GeoHealth, 7, e2022GH000690. https://doi.org/10.1029/2022GH000690

 
