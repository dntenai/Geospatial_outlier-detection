
**Data Import and Overview:**
I imported the dataset and conducted an initial overview to understand its structure and contents.

**Creating an Address Column:** 
I created an address column by concatenating fields such as State, LGA, Ward, and PU-Name to facilitate geocoding.

**Geocoding Function:**
I developed a geocoding function to fetch latitude and longitude coordinates using a service like Google Maps Geocoding API, ensuring accurate spatial data.

**Handling Missing Coordinates:**
I checked for missing values in latitude and longitude, removing rows with incomplete data to maintain data integrity.

**Neighborhood Identification:**
Using spatial analysis techniques, I identified neighboring polling units within a specified radius, crucial for subsequent outlier detection.

**Outlier Score Calculation:**
I implemented a function to compute outlier scores for each political party (e.g., APC, LP, PDP, NNPP) based on their voting patterns compared to neighboring units.

**Top 3 Outliers for Each Party:**
I generated reports showcasing the top 3 outliers for each party, detailing unit IDs, outlier scores, and the IDs of neighboring units contributing to their outlier status.

**Merge Outlier Scores:**
After calculating outlier scores, I merged this data back into the original dataset for comprehensive analysis

**Save Dataset:** I saved the enriched dataset, including outlier scores, to an Excel file located in a designated directory for further review and sharing.

**Findings**
***Top 3 outliers for APC:***

Unit ID: 27-05-08-006
Outlier Score: 409.00
Neighbours: [27-05-08-016, 27-05-08-023, 27-05-08-005]

Unit ID: 27-18-08-001
Outlier Score: 233.67
Neighbours: [27-18-08-006, 27-18-08-009, 27-18-08-008]

Unit ID: 27-08-11-006
Outlier Score: 222.80
Neighbours: [27-08-08-018, 27-08-11-015, 27-08-08-020, 27-08-08-016]

***Top 3 outliers for LP:***

Unit ID: 27-05-08-006
Outlier Score: 489.00
Neighbours: [27-05-08-016, 27-05-08-023, 27-05-08-005]

Unit ID: 27-20-02-012
Outlier Score: 189.79
Neighbours: [27-20-05-028, 27-20-02-006, 27-20-10-025, 27-20-02-004]

Unit ID: 27-05-08-005
Outlier Score: 171.00
Neighbours: [27-05-08-006, 27-05-08-016, 27-05-08-023]

***Top 3 outliers for PDP:***

Unit ID: 27-16-07-020
Outlier Score: 503.33
Neighbours: [27-16-07-015, 27-16-07-016, 27-16-07-026]

Unit ID: 27-16-07-023
Outlier Score: 350.00
Neighbours: [27-16-07-024, 27-16-07-021, 27-16-07-025]

Unit ID: 27-16-07-026
Outlier Score: 332.00
Neighbours: [27-16-07-020, 27-16-07-015, 27-16-07-016]

***Top 3 outliers for NNPP:***

Unit ID: 27-16-07-018
Outlier Score: 109.33
Neighbours: [27-16-07-020, 27-16-07-019, 27-16-07-017]

Unit ID: 27-16-07-020
Outlier Score: 87.33
Neighbours: [27-16-07-015, 27-16-07-016, 27-16-07-026]

Unit ID: 27-16-07-023
Outlier Score: 84.33
Neighbours: [27-16-07-024, 27-16-07-021, 27-16-07-025]

The above analysis highlighted potential anomalies guiding  investigation.
