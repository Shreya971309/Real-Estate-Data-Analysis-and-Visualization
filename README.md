<h1>Noida's Housing Market Insight - Power BI Dashboard </h1>


## Project Overview
(click to expand)

This Power BI project aims to offer comprehensive insights into the dynamic housing market of Noida, India. With a dataset comprising approximately 2300 property listings scraped from a leading real estate website, the dashboard provides users with a powerful tool to analyze market trends, pricing dynamics, and segmentation within Noida's housing sector.


## Project Structure
(click to expand)

<details>
<summary>   Data Collection and Cleaning </summary>
   
### Data Collection and Cleaning


## Data Collection

Data was collected using Python through API scraping, resulting in a dataset with the following fields:

- Property ID
- URL
- Price
- Price per Square Foot
- Bedroom Count
- Carpet Area
- Developer Name
- Location SEO Name
- Project Name
- Geographical Coordinates
- Possession Status
- Ownership Type
- Transaction Type
- Floor Number
- Number of Balconies
- Number of Bathrooms
- Furnishing Details
- Facing Direction
- Additional Room Details
- Availability Date
- Prime Location Indicator
- Luxury Amenities
- Property Title
- City Name

### Cleaning Process

During the cleaning process, several steps were undertaken:

- **Missing Values Handling**: Rows with missing price information were removed. For other columns, missing values were addressed using a combination of techniques such as imputation based on adjacent columns, interpolation, and manual verification.
  
- **Standardization of Units**: Area measurements were initially provided in different units (e.g., square meters, square yards). These units were standardized to square feet to maintain uniformity across the dataset.

- **Data Verification**: Discrepancies and unrealistic values were identified through careful verification using domain knowledge, external sources, and logical assessments. Erroneous values were corrected or flagged for further investigation.

The final dataset includes the following columns:

- Area
- Balconies
- Bathroom
- BHK (Bedroom, Hall, Kitchen)
- Developer Name
- Floor No.
- Furnished Status
- Latitude & Longitude
- Location
- Possession Status
- Price & Price per sq feet
- Project Name
- Property Type
- Segment (Derived)
- Transaction Type




</details>



<details>
<summary>   Data Transformation and Visualisation </summary>
   
## Data Loading and Transformation

#### Transformation Steps 

In Power BI, various transformations were applied to the dataset, including:

- **Segment Creation**: Utilizing DAX expressions, a custom segment was derived based on the price per square foot.
- The segmentation categorizes properties into three groups based on the criteria adopted from the real estate website 99acres:

-Premium: Properties with a price per square foot of 6000 or higher.
-Affordable: Properties with a price per square foot of 5000 or lower.
-Mid-Segment: Properties with a price per square foot between 5000 and 6000.

### Dashboard Components

#### Overview Page

The overview page features an assortment of interactive elements, including:

- **Average Price Card**: Providing a snapshot of the mean property price in Crores.
- **Average Price Per Sq Feet Card**: Displaying the average price per square foot.
- **Property Prices by BHK**: A horizontal bar chart segmented by BHK configuration, offering insights into the distribution of prices across different property types.
- **Transaction Type Pie Chart**: Illustrating the proportion of resale vs. new properties. 
- **Segment Pie Chart**: Depicting the distribution of properties across market segments (e.g., 'Premium', 'Affordable', 'Mid-Segment')
- **Segmentation by Possession Status**: A pie chart showing the proportion of Ready to Move vs. Under Construction properties.
- **Developer and Project Price Lists**: Presenting property prices alongside developer/project names with shaded price columns, allowing users to compare pricing across different projects and developers.
  - The shading in the price column of the developer and project tables forms a gradient based on the corresponding price per square foot. Darker shades represent higher 
    prices per square foot, gradually transitioning to lighter shades for lower prices per square foot. This gradient provides users with a clear visual indication of price 
    variations across properties.
- **Parameters: Average Price/ Average Price per Sqft**: Users can toggle between these parameters, influencing the data displayed on the charts accordingly. 
- **Filters:**
  - BHK configuration
  - Area range
  - Location within Noida
  - Market segment

- **Clear Filters Button**: A user-friendly feature enabling the reset of dashboard filters to default settings, enhancing usability and navigation.

<img width="647" alt="image" src="https://github.com/Shreya971309/Real-Estate-Data-Analysis-and-Visualization/assets/156785157/fc4a6cf9-b05e-444e-9487-0be47d296a2a">


#### Map Page

The map page offers a geospatial perspective of the Noida housing market, featuring:

- **Bubble Map**: Displaying locality markers sized by average price or price per square foot. This allows spatial analysis and identification of hotspots.
- **Filters and Parameters**: Similar to the overview page, enabling users to drill down into specific localities and explore detailed insights tailored to their needs and preferences.
<img width="649" alt="image" src="https://github.com/Shreya971309/Real-Estate-Data-Analysis-and-Visualization/assets/156785157/c84d598e-af2a-4cb6-9272-c66f9734703b">

  
</details>
  
<details>
<summary>  Insights and Observations </summary>

## Insights and Observations

#### Average Price and Average Price Per Sq Foot
- The average price of properties in Noida stands at ₹1.27 Crore, with an average price per square foot of ₹7,637.
- Among various configurations, 5BHK properties command the highest average price at ₹4.62 Crore, followed by 3BHK properties dominating the housing sector with an average price of ₹1.50 Crore. Meanwhile, 2BHK properties average at ₹66 lakhs, and 1BHK properties at ₹28 lakhs.

#### Transaction Type
- Resale properties dominate the market, constituting 87.64% of transactions, while new properties account for only 12.36%. This dominance of resale transactions suggests a mature market with a higher turnover of existing properties.

#### Possession Status
- The majority of properties (84.79%) are ready to move, indicating a preference among buyers for properties that are completed and available for immediate occupancy. Only 15.21% of properties are under construction.
- This preference for ready-to-move-in properties could stem from buyers' desire for immediate occupancy, assurance of quality, and the avoidance of potential construction delays commonly observed in the Noida market.

#### Prices of Projects
- Prices of projects vary widely, with some luxury projects commanding prices as high as ₹9.42 Crore. Most luxury project developers tend to focus on a single flagship project.


#### Localities
- Certain localities such as Sector 15, Golf Course, Sector 94, and Sector 43 command some of the highest prices per square foot, indicating premium locations with high demand.
- On the other hand, localities like Sector 87, 88, and 89 are on the lower end.

    </details>


    ## Files Included

 **Dashboard as PBIX**: [Noida Housing Dashboard.pbix](Noida%20Housing%20Dashboard.pbix) - Power BI dashboard file.
<br> **Dashboard as PDF**: [Noida Housing Dashboard.pdf](Noida%20Housing%20Dashboard.pdf) - PDF format of the Power BI dashboard.
<br> **Python Script for Data Scraping**: [Real_estate_scarping.ipynb](Real_estate_scarping.ipynb) - Jupyter Notebook containing Python script used for scraping real estate 
   data.
<br> **Pre-cleaned Data**: [property_listings_noida.xlsx](property_listings_noida.xlsx) - Excel file containing the raw data before cleaning.
<br> **Cleaned Data Loaded to Power BI**: [clean_prop_powerBI.xlsx](clean_prop_powerBI.xlsx) - Excel file containing cleaned data loaded into Power BI.





