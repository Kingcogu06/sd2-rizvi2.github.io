# Implementation

## Introduction
This web application lets users look up food businesses in Bristol and check their Food Hygiene Rating. By typing a business name into the search bar, the app sends a live request to the Bristol Open Data API and returns any matching businesses, along with their rating and the date they were last inspected.

The information comes from the Bristol Open Data portal, which publishes data collected by Bristol City Council as part of the national Food Hygiene Rating Scheme (FHRS). The scheme is run by the Food Standards Agency and enforced by local authorities. The dataset includes a wide range of  Bristol—restaurants, cafés, takeaways, supermarkets, and other places that handle food. Each entry includes the business name, a hygiene rating from 0 to 5, and the date of the most recent inspection. These three fields (BUSINESS_NAME, RATING, and RATING_DATE) are the ones the application  displays. 

There are a few limitations worth noting. The ratings shown are based on the most recent inspection recorded in the dataset, but the data may not always show the  latest inspection if updates haven’t yet been published. Some entries also contain missing or null values, which can lead to incomplete results. The dataset only covers businesses within the Bristol local  area, so anything outside that  won’t appear. To keep the interface simple, the app limits results to the first 20 matches, so additional businesses beyond that won’t be shown. Finally, the application needs to be run from a web server (such as GitHub Pages or VS Code Live Server).

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

![Insert your component Diagram here](images/component.png)

## Bristol Open Data API
TODO: Document each query to Bristol Open Data

![UML Class diagrams representing JSON query results](images/class1.png)
TODO: Repeat as necessary

# User guide
TODO: Explain how each use-case works by providing step-by-step screenshots for each use-case. This should be based on a tested scenario.
