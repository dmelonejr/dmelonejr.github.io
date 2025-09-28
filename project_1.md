## Project 1 - Park Candidate Parcels

**Project description:**  
Information for this project description was generated from the Project 1 Submittal document developed for course GIS-5013-999 taken Fall 2024 2025 in pursuit of a Geospatial [...]

### 1. Background

The GIS deliverable for this project should include data relating to a recommendation for the county on potential parcel candidates for purchase. These parcels must meet the following criteria: they m[...]

### 2. Criteria

* _The parcel must be vacant_:  
  Vector layer `vacant_parcels` can be utilized for this project. This layer can be used to help filter out the other data. Use "Select by Attributes" to filter the data by looking for parcels that match [...]

* _The parcel must be within walking distance of the LA River_:  
  Buffer 0.75 US Survey Miles around the LA River polyline layer.

* _The parcel must be far enough away from existing parks to avoid constructing redundant parks_:  
  Buffer 0.25 US Survey Miles from existing park parcels to reduce redundancy.

* _The parcel must be in an area with high population density_:  
  Layer: `block_groups` will provide the necessary data on population density greater than 8,000 people per square mile. Calculate the population density field and filter by the criteria.

* _The parcel must be in an area with a low median income_:  
  Layer: `block_groups` will provide the necessary data on median income by looking at `MDHINC_CY.` Use this number to filter out the criteria in the analysis.

* _The parcel must be in an area with a high population of children_:  
  Layer: `block_groups` will provide the necessary data on children less than or equal to the age of 18 under the data `POP18UP_CY`.

### 3. A note on LA Counties Census Block Data with "zero" values

These census block groups may contain buildings or land uses inconsistent with residential land use types. For example, the entire tract may encompass commercial buildings, stadiums, schools, parks, o[...]

### 4. Operational Steps

**Step 1:**  
Data Organization: I like to get my data organized. As this is unfamiliar data, my method is quite linear. I set up layer groups in the contents pane to act as containers for all the original data and [...]

![Step 1](images/Step%201_01.png?raw=true)

**Step 2:**  
After organizing the data and creating containers for my steps, I used a spatial join to combine the `block_groups` layer with the `vacant_parcels` layer.

**Step 3:**  
I created new fields and calculated the acres as all the area units are square feet in size. (To calculate the population density, the percentage of children, and then the child population must be calculated through subtraction – take the field for the age over 18 and subtract it from the [...]

**Step 4:**  
Once again, I utilized the Select by Location function from the toolbar to filter down the data to parcels, not within 0.25 miles of existing park polygons. On the menu's bottom is an option to invert [...]

**Step 5:**  
Each parcel was verified to be located within a census block (BLKGRP).

**Step 6:**  
The final step used the Select by Attributes function to narrow the vacant parcel data down to greater than or equal to 1 acre. As this map frame is in feet, I queried the data with the square footage [...]

### 5. Identify the parcels for potential parks

My analysis method derived four parcels that matched the search criteria. Their numbers are:

- 120B161-82
- 210B193-150
- 180B141-895
- 129A217-176

### 6. Conclusion

In summary, I used tools I was comfortable with from our lessons during the course to date. I found that with my analysis style, breaking these steps into condensed queries helped put my mind at ease [...]

### 7. Appendix

Location Map:

![Location Map](images/Layout.jpg?raw=true)

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).
