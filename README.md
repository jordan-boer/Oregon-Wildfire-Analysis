# Oregon-Wildfire-Analysis
Career Foundry project using Python and Tableau to analyze historical wildfire data in Oregon from 2000-2022. The aim is to identify the main causes and high risk areas in the state in order to increase prevention and reduce damage.
## Project Overview
In the state of Oregon, wildfires are an ever present problem with hundreds of fires devastating forests, homes, and businesses each year. According to the World Health Organization, climate change is creating warmer temperatures and drier conditions leading to longer fire seasons. While small wildfires can be good for a forest's overall health, recent wildfires are becoming more extreme in terms of acres burned, duration, and intensity. This leads to negative environmental impacts such as the release of large quantities of carbon dioxide and other greenhouse gases into the atmosphere creating a reduction in air quality for surrounding populations. In addition to the immediate damage to residences and businesses, wildfires can also affect populations indirectly by disrupting transportation, communications, water supply, and power and gas services. 
## Key Questions
- What area of Oregon has the most wildfires?
- What is the main cause of wildfires?
- Is there a correlation between the total number of acres burned and the number of protected acres burned?
- Is the number and intensity of wildfires increasing, decreasing, or staying the same over time?
## Folders
Content description of project folders:
- 01 Project Management: contains the project brief that outlines the details of the project.
- 02 Data: contains two subfolders:
  - Original Data: contains the original datasets of the project (one .csv file and one .geojson file).
  - Prepared Data: contains the final cleaned and wrangled dataset used for analysis.
- 03 Scripts: contains Jupyter notebooks of each step of my analysis written in Python code.
- 04 Analysis-Visualizations: contains all the visualizations I created to develop and explain insights.
## Data
Original data set used for this analysis and columns they contain:
- fire_occurrence: Serial, FireCategory, **FireYear**, **Area**, **DistrictName**, **UnitName**, FullFireNumber, **FireName**, **Size_class**, **EstTotalAcres**,
    **Protected_Acres**, **HumanOrLightning**, **CauseBy**, **GeneralCause**, SpecificCause, Cause_Comments, **Lat_DD**, **Long_DD**, LatLongDD, **FO_LandOwnType**,
    Twn, Rng, Sec, Subdiv, LandmarkLocation, **County**, RegUseZone, RegUseRestriction, Industrial_Restriction, **Ign_DateTime**, **ReportDateTime**,
    **Discover_DateTime**, **Control_DateTime**, CreationDate, ModifiedDate, DistrictCode, UnitCode, DistFireNumber.

  *Note: Bold columns are the ones I used for analysis and some columns name were changed for clarity and consistency.
- county_boundaries: a GeoJSON file that includes point locations for plotting maps in Python.
## Tools
Code was written in Jupyter notebooks using Python and utilizing the following libraries:
- Pandas: for data manipulation and analysis
- NumPy: for mathematical functions
- OS: for reading/writing files and navigating file system
- Matplotlib.pyplot: for creating visualizations
- Seaborn: for more advanced statistical data visualizations
- Folium: for plotting interactive maps
- SKLearn: used modules for various analyses such as linear regression, calculating mean_squared and r2 score, and kmeans
- Pylab: for simplified plotting and numerical calculations
- Statsmodels.api: for testing stationarity and autocorrelation
## Tableau Storyboard
Link for my final results of analysis. Does not contain every step of analysis, only those relevant to final results.
https://public.tableau.com/app/profile/jordan.boer/viz/OregonWildfireAnalysis/Story1?publish=yes
## Sources
 - fire_occurrence.csv data set was accessed from https://www.kaggle.com/datasets/mattop/fire-occurrence-and-cause-data-2000-2022/data?select=fire-occurence.csv via Kaggle
 - county_boundaries.geojson data was accessed from https://geohub.oregon.gov/datasets/oregon-geo::county-boundaries/explore?location=45.170334%2C-120.662000%2C5.54 via Oregon.gov

   Both originally created by the Oregon Department of Forestry - https://data.oregon.gov/Natural-Resources/ODF-Fire-Occurrence-Data-2000-2022/fbwv-q84y/about_data
