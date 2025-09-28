## Project 1 - Park Candidate Parcels

**Project description:** Information for this project description was generated from the Project 1 Submittal document developed for course GIS-5013-999 taken Fall 2024 2025 in pursuit of a Geospatial Technologies Master's from the University of Oklahoma.

### 1. Background

The GIS deliverable for this project should include data relating to a recommendation for the county on potential parcel candidates for purchase. These parcels must meet the following criteria: they must be vacant, within a high population density, and in an area with below-average median income. The deliverable should include a map(s) and a written summary of the parcel IDs, general location attributes (population demographics), and value.

### 2. Criteria

<em>The parcel must be vacant</em>: \
Vector layer "vacant_parcels" can be utilized for this project. This layer can be used to help filter out the other data. Use "Select by Attributes" to filter the data by looking for parcels that match the area criteria greater than or equal to one acre. \
\
<em>The parcel must be within walking distance of the LA River</em>: \
Buffer 0.75 US Survey Miles around the LA River polyline layer. \
\
<em>The parcel must be far enough away from existing parks to avoid constructing of redundant parks</em>: \
Buffer 0.25 US Survey Miles from existing park parcels to reduce redundancy. \
\
<em>The parcel must be in an area with high population density</em>: \
Layer: "block_groups" will provide the necessary data on population density greater than 8,000 people per square mile. Calculate the population density field and filter by the criteria. \
\
<em>The parcel must be in an area with a low median income</em>: \
Layer: "block_groups" will provide the necessary data on median income by looking at "MDHINC_CY." Use this number to filter out the criteria in the analysis. \
\
<em>The parcel must be in an area with a high population of children</em>: \
Layer: "block_groups" will provide the necessary data on children less than or equal to the age of 18 under the data "POP18UP_CY").

### 3. A note on LA Counties Census Block Data with "zero" values:

These census block groups may contain buildings or land uses inconsistent with residential land use types. For example, the entire tract may encompass commercial buildings, stadiums, schools, parks, or other non-residential land use types.

### 4. Operational Steps:

<em>Step 1:</em> \
Data Organization: I like to get my data organized. As this is unfamiliar data, my method is quite linear. I set up layer groups in the contents pane to act as containers for all the original data and then any output data. I then symbolize the data for legibility. \
\
<img src="images/Step 1_01.png?raw=true"/>
\
<em>Step 2:</em> \
After organizing the data and creating containers for my steps, I used a spatial join to combine the "block_groups" layer with the vacant_parcels layer. \
\
<em>Step 3:</em> \
I created new fields and calculated the acres as all the area units are square feet in size.
(To calculate the population density, the percentage of children, and then thee child population must be calculated through subtraction – take the field for the age over 18 and subtract it from the total population in 2010. This should provide the requisite data. \
\
<em>Step 4:</em> \
\
Once again, I utilized the Select by Location function from the toolbar to filter down the data to parcels, not within 0.25 miles of existing park polygons. On the menu's bottom is an option to invert the spatial relationship. This enabled the inverse of the relationship "within a distance" of 0.25 miles. \
\
<em>Step 5:</em> \
Each parcel was verified to be located within a census block (BLKGRP). \
\
<em>Step 6</em> \
\
The final step used the Select by Attributes function to narrow the vacant parcel data down to Greater than or Equal to 1 acre. As this map frame is in feet, I queried the data with the square footage of 43,560 (equal to 1 acre).

### 5. Identify the parcels for potential parks: \

My analysis method derived four parcels that matched the search criteria. Their numbers are: \
•	120B161-82 \
•	210B193-150 \
•	180B141-895 \
•	129A217-176 \

### 6. Conclusion

In summary, I used tools I was comfortable with from our lessons during the course to date. I found that with my analysis style, breaking these steps into condensed queries helped put my mind at ease that I was using the correct tools. I believe this approach satisfies the client's analysis requirements. I verified data along the way (looked at a buffer along the river and buffers along park boundaries) to ensure that data satisfied the criteria. Outside of urban planning, this approach (or others with the tools we've learned) can be used to locate pipes in a stormwater network for repair and replacement or provide additional metropolitan planning for transportation infrastructure. This type of analysis can also look at elevation data and soil types to compare existing and proposed conditions from survey and digitized map data.

### 7. Appendix

Location Map:

<img src="images/Layout.jpg?raw=true"/>

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).
