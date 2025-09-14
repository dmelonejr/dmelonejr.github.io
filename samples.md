## This can be your internal website page / project page

**Project description:** Information for this project description was generated from the Project Proposal document (memorandum) developed for course GIS-5253-999 taken Summer 2025 while in pursuit of a Geospatial Technologies Master's from the University of Oklahoma.

### 1. Background

During the Summer GIS-5253-999 GIS Applications course, students were introduced to a variety of lab assignments to enhance their understanding of different types of projects and tools available to them, thereby increasing their knowledge and comprehension of spatial data and various data interpretation techniques. One such lab assignment focused on spatial interpolation. During this lab assignment, students used temperature data to examine variations in analysis techniques for temperatures across the state of Texas.
Inspired by that lab assignment, this project proposal aims to review soil temperature data collected at the same sites. The overall objective is to utilize current data to lay the groundwork for an analysis process that interprets a variety of natural data. Using the analysis methods described in the mentioned lab assignment, the analyst aims to determine if there is a similar distribution in temperature variation throughout the various soil sample depths versus the interpolated air temperature data. Rainfall data could be included in this dataset at a later time to expand the examination of temperature variation distribution across the study area. To summarize, this exercise aims to apply analysis techniques established throughout the semester, empowering analysts to make the best-informed decisions with available data and identify any similar trends in air and below-surface temperatures in Texas.

### 2. Method

1.	Unit of Analysis. Units for this project will remain the same as the input datasets. Temperature data is recorded in degrees Fahrenheit, and soil temperature is measured in degrees Fahrenheit at centimeters below grade. The scope of this project encompasses the entire state of Texas, including all Texas Water Development Board (TWDB) data recording and monitoring stations.
2.	Data and Sources. Data was compiled from the TexMesonet website for analysis on June 19, 2025. According to the TexMesonet website (https://www.texmesonet.org/About), data is compiled in collaboration with various stakeholders by the Texas Water Development Board (TWDB). Stations are maintained by the National Weather Service (NWS), as well as various regional and local entities. The projected coordinate system for the data and maps shall be WGS 1984 UTM Zone 14N.
3.	Techniques. The TWDB_Mesonet_Stations point layer from Lab 4 will be utilized to combine the temperature and rainfall data downloaded on June 19th, 2025. After joining the data, the environment shall be set to the state of Texas polygon utilized from the Lab 4 dataset. All data will be joined together using a common identifier. Temperature data will then be analyzed using the Kriging spatial analysis method at the various depths available, and the data will be clipped to the state boundary. The analyst will create multiple maps to display soil temperature trends across the state. Each of these maps will empower the analyst to provide their interpretation of the data at the time of collection.

### 3. Assumptions

This project assumes that all data available online is current within an acceptable parameter. The purpose of this project is to demonstrate accurate data collection, analysis, and summary. It is assumed that this assignment provides students with the opportunity to learn and grow in their academic possibilities and is not necessarily a reflection of an actual research project or one that any company or municipality is undertaking. It is also assumed that any information derived from this study is no reflection on the data owners or facilitators.

### 4. Limitations

Every project contains limiting factors – addressing issues that require attention to public data is one such potential pitfall. Any analysis for public use cases will inherently include stumbling blocks. Limitations may include access to data sources, the accuracy of online sources, and the dates of data collection. Limitations for this project also include a shortened timeline and the importance of the initial research project.

### 5. Work Plan

1.	Phase I: Identify the project scope and data [05/25]
  a.	Consider the problem that requires answering
  b.	Identify study area/limit in scope for success
  c.	Collect data and aggregate for usage
2.	Phase II: Analyze compiled data and interpret results [06/25]
  a.	Import and combine necessary data for analysis
  b.	Create an air temperature map
  c.	Create soil temperature maps at the available depths (e.g., 5 cm) using the same analysis methodology.
3.	Phase III: Deliverables [06/25]
  a.	Oral presentation of the findings online in a three-minute speech format
  b.	Create and submit an ArcGIS StoryMap to the best possible standard, given the scope of this course and expectations in an accelerated summer session.

### 6. Conclusion

It is logical to assume higher air temperatures statewide potentially indicate identical results in soil temperature at various depths. The purpose of this exercise is to compare the distribution and interpolation of data across the state, given the results of the in-class lab. It is safe to assume that the analyst understands a variety of soil types exist across the vast geography of any state and may affect the readings. The purpose of this exercise is to determine if there is any difference across the state, given the varying measurement depths. This process may lead to additional testing that includes soil types at a more micro level of analysis, allowing for a more precise interpretation.

### 7. Reference

“TexMesonet.” TexMesonet, 2025, www.texmesonet.org/DataProducts/TWDBStations/SoilMoisture. Accessed 19 June 2025.
“TexMesonet.” TexMesonet, 2025, www.texmesonet.org/About. Accessed 19 June 2025.

### 8. Appendix

Location Map



# For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).
