# Noida Housing Market Insight

## Overview

This Power BI project aims to provide comprehensive insights into the housing market in Noida, India, using data scraped from a popular real estate website. The project encompasses data cleaning, analysis, and visualization to offer users a clear understanding of property prices, market segments, transaction types, and construction statuses in Noida.

## Project Components

### Data Collection and Cleaning

1. **Data Collection**:
   - Scraped data from a real estate website using API scraping, resulting in a dataset containing information on approximately 2300 property listings.
  
2. **Data Cleaning**:
   - Identified missing values across different columns, such as price, area, developer name, project name, and others.
   - Rows with missing values in crucial columns like price were deleted to ensure data integrity and accuracy.
   - For columns with a high number of missing values:
     - Used adjacent columns or similar listings to infer missing values.
     - Conducted Google searches to fill in missing information where possible.
     - Manually checked and corrected discrepancies and absurd values based on external sources or domain knowledge.
   - Standardized units of measurement for area (e.g., sqm, sqyard) to square feet for consistency.
   - Applied conversion factors to convert area measurements to a standard unit, ensuring uniformity across the dataset.
   - Detected discrepancies and absurd values in various columns, such as price, area, and property attributes.
   - Conducted Google searches and cross-referenced with project details to verify the accuracy of values.
   - Corrected or removed values that did not align with the expected ranges or were deemed unrealistic.
   - Created calculated columns such as price per square foot and a custom segment based on price per square foot to categorize properties into premium, affordable, and mid-segments.

### Data Analysis and Visualization

1. **Loading to Power BI**:
   - Once the data cleaning process was completed, the refined dataset was loaded into Power BI for further analysis and visualization.

2. **Creating Visualizations**:
   - Developed various visualizations to represent key insights:
     - Average price and price per square foot cards
     - Property prices by BHK configuration
     - Distribution of properties by transaction type
     - Distribution of properties across market segments
     - Lists of developer names and project names with corresponding prices, shaded based on price per square foot
     - Segmentation by transaction type
   - Implemented filters for refining data based on price range, BHK configuration, area, location, and property segment.

### Interactive Map Visualization

1. **Creating Map Page**:
   - Created a second page with a bubble map visualization of different localities in Noida, marked using latitude and longitude coordinates.
  
2. **Bubble Map**:
   - Bubble sizes correspond to average price or price per square foot, providing users with a spatial understanding of property prices across different areas.
  
3. **Filters and Parameters**:
   - Implemented similar filters and parameters as on the first page to enable users to drill down into specific localities and explore detailed insights.

## Insights and Observations

Based on the analysis conducted through the Power BI dashboard, the following insights and observations were made:

1. **Average Prices**: The average price of properties in Noida is ₹1.26 Crores, with an average price per square foot of ₹7,626.
  
2. **Property Prices by BHK**: Property prices vary significantly based on the configuration of bedrooms, halls, and kitchens, indicating a diverse market with properties ranging from affordable to luxury.
  
3. **Market Segmentation**: The majority of properties fall within the premium segment category, followed by the affordable and mid-segments, reflecting the diversity of offerings in the market.
  
4. **Transaction Types**: Resale properties dominate the market, accounting for the majority of transactions, while new properties constitute a smaller portion, suggesting a mature market with a preference for established properties.
  
5. **Construction Status**: A significant majority of properties are ready to move in, indicating a preference for completed properties among buyers.
  
6. **Developer and Project Pricing**: The availability of properties across different price points suggests a range of options for buyers, with the highest-priced project being Estate 128 by Max Estate Developers.

## How to Use

1. **Opening the Dashboard**: Open the Power BI file provided using Power BI Desktop or Power BI Service.
  
2. **Navigating Pages**: Use the navigation buttons or tabs to switch between the overview page and the map page.
  
3. **Exploring Insights**: Utilize the interactive elements such as filters, slicers, and parameters to refine the data and explore specific insights tailored to your requirements.
  
4. **Interacting with Visualizations**: Hover over data points or click on elements within visualizations to view detailed information or apply filters dynamically.
  
5. **Drilling Down**: On the map page, right click on bubbles representing different localities to drill down into specific areas and view localized insights.



## Disclaimer

This project is for demonstration purposes only and does not constitute financial or investment advice. All data presented is based on publicly available information and should be verified independently.

