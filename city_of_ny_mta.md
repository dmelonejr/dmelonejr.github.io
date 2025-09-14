## Soil Temperatures at Depth - Data Interpolation Fundamentals

**Project description:** Information for this project description was generated from the Project Proposal document (memorandum) developed for course GIS-5253-999 taken Summer 2025 while in pursuit of a Geospatial Technologies Master's from the University of Oklahoma.

### 1. Background

During the Summer GIS-5653-999 Spatial Programming and GIS course, students were introduced to a variety of lab assignments to enhance their understanding of Python programming and the integration with ArcGIS and other spatial analysis applications. After researching a unique project for this proposal, this project proposes to combine the data found on the Data.gov website for major incidents on subways from the Metropolitan Transit Authority in the City of New York. This data is important as it shows locations where significant delays occurred which impacted riders. This project is proof of concept for the author of this memorandum – proving the processes learned in this class (and others) are applicable to this type of data analysis. The final presentation should include the python code potentially in the Jupyter Notebook format as well as a mapping offering for visualization and proof that the analysis worked. Ideally, to prove user-interactivity, it would be beneficial to include a user-input function to call incidents for specific stations. It is believed that this type of analysis is typical to provide to decisions makers when looking at infrastructure problem areas for public transit and planning.

### 2. Keywords

•	Metropolitan Transit Authority
•	State of New York
•	Subway
•	Mass transit
•	Service disruption
•	delay

### 3. Data Requirements

Potential data sources, broadly speaking, include:
1.	Required input data
  a.	MTA Subway Major Incident
  b.	Census TIGER/Line census block data
  c.	Subway station locations
  d.	City of New York boundary data
2.	Data Sources
  a.	MTA Subway Major Incidents from data.gov
  b.	US Census TIGER/Line data from census.gov
  c.	State of New York MTA Subway Stations locations from data.ny.gov
3.	Data type (raster, vector, point, line, polygon)
  a.	Tables
  b.	Points
  c.	Polygons

### 4. Process Description

1.	Phase I: combine data inside ArcGIS Pro and Python. 
  a.	Loop through the data during analysis with several types of criteria (i.e. look at the data and present different levels of the data: no incidents, up to twenty incidents, up to fifty incidents, greater than fifty incidents).
  b.	Do not include data in the final map that is under a certain threshold after reviewing the significant incidents throughout the MTA’s jurisdiction.
  c.	ArcGIS processes include:
    i.	AddField, ListFeatureClasses, clip_features, arcpy.env.workspace, RefreshLayer, ListFields
2.	Phase II: narrow down and clip data by the census block data with the most frequent incidents over the study time.
  a.	Clipping can be completed through Python (like in Exercise 8) and checked within ArcGIS Pro.
  b.	Join data appropriately from disparate sources.
  c.	Data should be symbolized appropriately for this analysis.
3.	Phase III: ensure the data is represented on a map appropriately.
  a.	Display incident data with some kind of appropriate symbology (small to large circles, etc.)
  b.	Show census block polygons with labels on the map that contain the incident categories outlined briefly above (may need to adjust this categorization after working throught the data)

### 5. Reference

•	“Data.gov.” Data.gov, 2020, catalog.data.gov/dataset/mta-subway-major-incidents-beginning-2020. Accessed 27 July 2025.
•	US Census Bureau. “TIGER/Line Shapefiles.” The United States Census Bureau, 6 May 2019, www.census.gov/geographies/mapping-files/time-series/geo/tiger-line-file.html.
•	“MTA Subway Stations | State of New York.” Data.ny.gov, data.ny.gov/Transportation/MTA-Subway-Stations/39hk-dx4f/about_data

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).
