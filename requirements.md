# Requirements
## Functional Requirements 
The Functional Requirements that the food hygiene app have are:
* Search functionality -> Users are able to search for food businesses by name, location or cuisine.
* Food hygiene ratings -> Display offical food hygiene scores.
* Inspector details -> Show inspection data e.g. date, reason and notes.
* Map integration -> Interactive apps to locate nearby business with ratings and filters.
* Customer reviews and photos -> Allows customers to share personal expereinces which are seperate from the hygiene data.
* Report a problem -> To report issues or suspected hygiene violations to relevant authority.
### Non-Functional Requirements
The Non-Functional requirements are:
* Usablity -> Simple design for easy use for all ages.
* Performance -> Fast loading of search results and data for said results.
* Scalablity -> Handle large datasets for the food businesses.
* Reliablity -> Data should be accurate and updated frequently.
* Compatiblity -> Available on IOS, Android and web platforms.
* Accessiblity -> Meet accessiblity standards.
* Screen size --> Must accommodate all screen sizes for the device that is being used.

## User Needs

#### User stories
As a User, I want to search for food hygiene ratings by business name, location or rating so I am able to make a good choice about where to eat.

As a User, I want the application to suggest nearby businesses if my search returns with no results so I can find alternatives. 

As a User, I want to filter search results by rating so I can identify businesses with a high standard of food hygiene.

As a User, I want to report any food safety issues through the application so I can alert authorities to the risks the business is accommodating.

As a User, I want the application to be accessible on mobile devices so that it can be used on the move. 

As a User, I want to recieve confirmation after submitting a report so I know my submission was successful.

As a User, I want the application to detect my location and for the application to show nearby businesses.

As a User, I want to view hygiene ratings in a list format so I can quickly scan multiple businesses without using the geolocation feature.

As a User, I want to naviagte through pages when there are many results so I can explore more options.

As a User, I want to see the total of businesses listed so I know how many options are available.

As a Business Owner, I want to be proud of hygiene rating as it would encourage more people to visit the business.

As a Inspector, I want to be able to look at old results and enter a business with expectations.

As a Inspector, I want to be able to decrease the amount of paper used in documenting hygiene in these businesses.

As a Inspector, I want to show my results publically while keeping parts of the result confidential for only the business owners to see.

As a Developer, I want to have access to Bristol Open Data API and implement it into the application to retrieve accurate food hygiene ratings for businesses.

### Actors
The actors and users for the food hygiene app will be:
* Users --> Consumers who want to view and search for food hygiene ratings for local food businesses/restaurants in Bristol to make decisions on where to eat and report any food related issues.
* Business Owners --> Food business owners in Bristol who want to access their information. The information that will be available on the application is the organisation's food hygiene rating, maintain their accurate information, request corrections and answer to reported incidents.
* Food Hygiene Inspector --> Inspectors come to businesses with expectations and make their reason for their grade publically which leave some things secret for only the business owner to see.
* Developer --> Responsible for creating and maintaining the database, managing corrections, handling appeals and making sure the app works properly and keeping data accurate from Bristol Open Data.

### Use Cases
| USE-CASE ID | UC1 | 
| -------------------------------------- | ------------------- |
| **Description** | Users can check food hygiene ratings, find trusted restaurants, and report any food safety problems. |
| **Actors** | Users which can be the general public or consumers |
| **Assumptions** | <ul><li> The user knows the name, location or rating of the restaurant.</li><li> The user is familair with how to use apps and knows how to use a search feature</li><li> The user is connected to a device which can be used by Wifi or using data, the phone must be connected by a satelite signal.</li><li> The food business must have a rating for it to show up on the application.
| **Steps** | **<br>1**- User opens the web or mobile application. **<br>2**- System uses goelocation to show nearby businesses in bristol **<br>3**- User uses the search feature. **<br>4**- User enters a search term, such as Business Name, Location (Street, District or Postcode), Cuisine or Hygiene Rating. **<br>5**- User selects a rating from 0-5 to define results. **<br>6**- User clicks the 'Search' button. **<br>7**- The system sends a request to Bristol Open Data API. **<br>8**- The system displays the serach results on the map with markers for the business correlating to the results. **<br>9**- User clicks a business marker to view the organisation's details. **<br>10**- If no results are found then the system suggests nearby businesses with the same rating. **<br>11**- User clicks the 'Show list' button to switch to the list view instead of depending on the geolocation feature. **<br>12**- The system fetches the data again from Bristol Open Data API. **<br>13**- The system then displays the Business Names and Locations. **<br>14**- The system shows the number of results ( e.g. 'Showing 1-10 of 4,753 results'. **<br>15**- If there are more than 10 results, the system adds a button at the end of the page with 'Next' and 'Previous'. **<br>16**- User can control the pages using these buttons and it says at the top (e.g.Page 1-342). **<br>17**- If no results are shown, then the system displays a message that says 'No results found'. **<br>18**- The system then adds to the page suggestions with what the users picked with their filters. |
| **Variations** | <ul><li> If no results are found, the app then shows a message saying, 'No Results Found' and suggests nearby businesses. </li><li> If used filters to search then the application should suggest businesses that correlate to the users' chosen filters. </li><li> The app displays nearby businesses in Bristol </li><li> If the user enters a partial name of a business, the application matches possible matches that matches the partial input.  |
| **Non-functional** | The search should return the reuslts as quick as possible to avoid the user waiting. The app was made so that users can make quick decisions.  |
| **Issues** | The system should have a backup source in case if Bristol Open Data API has downtime for some reason and if the servers are down it should let the user know so they are prepared for slower time in getting results. |


|USE-CASE ID | UC2 | 
| -------------------------------------- | ------------------- |
| **Description** | The business owner can verify that their food hygiene rating is accurate and if someone reports that their is incorrect rating, it is their responsiblity to fix the rating to make it accurate. |
| **Actors** | Business owners and Inspectors |
| **Assumptions** | <ul><li> The business owner has access to the food hygiene application and can look at reports to their business about their ratings. </li><li> The business owner's organisation already has an existing rating in the Bristol Open Data API database so they are responsible for updating when they have a better/lower rating. </li><li> Business owners can reply to reports to say that they are working on the issue that the report has brought to light.  |
| **Steps** | **<br>1** Business owner opens the application called GrubGrade. **<br>2** If geolocation is allowed, the map centres on the user's location and shows nearby businesses. **<br>3** Business owner uses the search feature. **<br>4** Business owner enters a search term, this can be a business name or location. **<br>5** The business owner applies a hygiene rating filter (0-5) if needed. **<br>6** System retrieves and displays results. **<br>7** Business owner confirms that the hygiene rating that is being displayed is accurate.**<br>8** If incoreect the business owner fills out the correction form and submits it. **<br>9** System confirms submission and notifies the business owner. |
| **Variations** | If the business isn't found in the application, the app then shows suggested/reccommended businesses nearby.  |
| **Non-functional** | <ul><li> The application should be available 24/7 365 days which allows consumers to report issues at anytime of the day.</li><li> The Business owners would then fix the reports as soon as posssible and can fix these anytime in the day so consumers wouldn't be confused with the inaccurate ratings. |
| **Issues** | The system must handle situations where business data is missing or outdated, this would then be fixed through the business owner to fix the inaccurate date from their end to resolve the issue. |


| USE-CASE ID | UC3 | 
| -------------------------------------- | ------------------- |
| **Description** | Food hygiene rating data can be implemented by developers via the Bristol Open Data API, with appropriate fallback and error-handling mechanisms. |
| **Actors** | Web/App developer|
| **Assumptions** | <ul><li> The developer should have access to the Bristol Open Data API and have necessary API credentials. </li><li> The API should function correctly and return data in the correct format for integration for the application.</li><li> The developer must be able to implement backup methods in case if the API fails.|
| **Steps** | TODO: Interactions between actors and system necessary to achieve goal |
| **Variations** | TODO: OPTIONAL - Any variations in the steps of a use case |
| **Non-functional** | Fallback data should be available without any noticeable delay if the primary database fails. |
| **Issues** | If both the API and the backup data fail, then the app/web application should display an error message and askes the user to try again later. |


TODO: Your Use-Case diagram should include all use-cases.

![Insert your Use-Case Diagram Here](images/use-case.png)
<img width="1920" height="2560" alt="image" src="https://github.com/user-attachments/assets/b79785e1-ae18-41d8-8ea0-d9e042569ed6" />


## Software Requirements Specification
### Functional requirements
TODO: create a list of functional requirements. 
    e.g. "The system shall ..."
    Give each functional requirement a unique ID. e.g. FR1, FR2, ...
    Indicate which UC the requirement comes from.


### Non-Functional Requirements
TODO: Consider one or more [quality attributes](https://en.wikipedia.org/wiki/ISO/IEC_9126) to suggest a small number of non-functional requirements.
Give each non-functional requirement a unique ID. e.g. NFR1, NFR2, ...

Indicate which UC the requirement comes from.
