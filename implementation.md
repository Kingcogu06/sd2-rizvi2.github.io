# Implementation

## Introduction
This web application lets users look up food businesses in Bristol and check their Food Hygiene Rating. By typing a business name into the search bar, the app sends a live request to the Bristol Open Data API and returns any matching businesses, along with their rating and the date they were last inspected.

The information comes from the Bristol Open Data portal, which publishes data collected by Bristol City Council as part of the national Food Hygiene Rating Scheme (FHRS). The scheme is run by the Food Standards Agency and enforced by local authorities. The dataset includes a wide range of  Bristol—restaurants, cafés, takeaways, supermarkets, and other places that handle food. Each entry includes the business name, a hygiene rating from 0 to 5, and the date of the most recent inspection. These three fields (BUSINESS_NAME, RATING, and RATING_DATE) are the ones the application  displays. 

There are a few limitations worth noting. The ratings shown are based on the most recent inspection recorded in the dataset, but the data may not always show the  latest inspection if updates haven’t yet been published. Some entries also contain missing or null values, which can lead to incomplete results. The dataset only covers businesses within the Bristol local  area, so anything outside that  won’t appear. To keep the interface simple, the app limits results to the first 20 matches, so additional businesses beyond that won’t be shown. Finally, the application needs to be run from a web server (such as GitHub Pages or VS Code Live Server).

## Dataset
The application uses a GeoJSON dataset:
- There is the Food_Hygiene_Ratings.geojson which contains the information about the businesses, their hygiene ratings and their inspection dates/reaosns for their score. This is the main dataset for the website.
- Backup_Food_Hygiene_Ratings.geojson is the backup dataset and this boots up when the main dataset has an error and is unavailable at the time. This lets the application to continue to function even though the main datasset fails. This allows the application to always run even though the main dataset has an error or fails.

## Limitations 
The limitations of the dataset are:
- A business could improve or decline after an inspection so the data may be outdated so their might be delays in logging in new hygiene ratings.
- Some businesses are inspected more than others as high risk businesses will gain more visits than low-risk ones. So the lower the hygiene score, the higher of frequency of inspections.
- Inspectors follow guidelines but judgement can vary between each food inspector, this introduces human bias as every thinks differently.
- Not all businesses are included as some businesses will be run from people's homes or can be temporary businesses such as food trucks.


## Project Structure

| File        | Role                                                                 |
|-------------|----------------------------------------------------------------------|
| index.html  | The main page of the application. Defines the structure and 
               content of the user interface, including the search input, 
               button, result card, and multiple results list.          |
| style.css   | Contains all visual styling for the application, including layout and 
               colours       |
| script.js   | Contains all JavaScript logic, including building and sending the API 
               query to Bristol Open Data, handling the JSON response, 
               and  updating the page with results or error 
               messages.   

               jslint warnings = 24

    
## Software Architecture
TODO: Describe the major components of your architecture. Are any particular architectural styles being used?
<img width="1059" height="297" alt="image" src="https://github.com/user-attachments/assets/f874ff53-c6d3-4d80-991b-598a23cc7c82" />


![Insert your component Diagram here](images/component.png)

## Bristol Open Data API
Our applicayion sources the dataset from the Bristol Open Data API. The dataset was downloaded as a Geojson file and is used as the primary dataset for the website. Consuners are able to search for businesses by:
- Search by business name as users can search for food businesses by entering their name. This allows users to gain hygiene ratings of a specific location.
- Filter by hygiene rating, users can filter results by hygiene ratings. This allows consumers to see businesses with a specific rating which makes it easier to focus on businesses that meet the users preferred expectations.
- Postcode search, by entering a postcode users are able to view businesses with hygiene ratings in a specific area. This feature allows to give users information for their area of interest.

To make sure the dataset does not fail, the webiste includes a backup data loading mechanism. If the primary dataset is unavailable then the application would load the data from backup json file. This backup option ensures that the app remains functional and is available 24/7 and 365 days a year.

![UML Class diagrams representing JSON query results](images/class1.png)
<img width="302" height="299" alt="image" src="https://github.com/user-attachments/assets/c91dd8e3-036d-43c8-9a4d-356f6e6278f7" />


# User guide
TODO: Explain how each use-case works by providing step-by-step screenshots for each use-case. This should be based on a tested scenario.
