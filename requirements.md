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
TODO: Describe each use case (at least one per team member).
    Give each use case a unique ID, e.g. UC1, UC2, ...
    Summarise these using the use-case template below.

| TODO: USE-CASE ID | UC1 | 
| -------------------------------------- | ------------------- |
| **Description** | Users can search for food hygiene ratings and find restaurants with good ratings or report a food safety issue. |
| **Actors** | Users which can be the general public or consumers |
| **Assumptions** | <ul><li> The user knows the name, location or rating of the restaurant.</li><li> The user is familair with how to use apps and knows how to use a search feature</li><li> The user is connected to a device which can be used by Wifi or using data, the phone must be connected by a satelite signal.</li><li> The food business must have a rating for it to show up on the application.
| **Steps** | **<br>1**- User opens the web or mobile application. **<br>2**- System uses goelocation to show nearby businesses in bristol **<br>3**- User uses the search feature. **<br>4**- User enters a search term, such as Business Name, Location (Street, District or Postcode), Cuisine or Hygiene Rating. **<br>5**- User selects a rating from 0-5 to define results. **<br>6**- User clicks the 'Search' button. **<br>7**- The system sends a request to Bristol Open Data API. **<br>8**- The system displays the serach results on the map with markers for the business correlating to the results. **<br>9**- User clicks a business marker to view the organisation's details. **<br>10**- If no results are found then the system suggests nearby businesses with the same rating. **<br>11**- User clicks the 'Show list' button to switch to the list view instead of depending on the geolocation feature. **<br>12**- The system fetches the data again from Bristol Open Data API. **<br>13**- The system then displays the Business Names and Locations. **<br>14**- The system shows the number of results ( e.g. 'Showing 1-10 of 4,753 results'. **<br>15**- If there are more than 10 results, the system adds a button at the end of the page with 'Next' and 'Previous'. **<br>16**- User can control the pages using these buttons and it says at the top (e.g.Page 1-342). **<br>17**- If no results are shown, then the system displays a message that says 'No results found'. **<br>18**- The system then adds to the page suggestions with what the users picked with their filters. |
| **Variations** | TODO: OPTIONAL - Any variations in the steps of a use case |
| **Non-functional** | TODO: OPTIONAL - List of non-functional requirements that the use case must meet. |
| **Issues** | TODO: OPTIONAL - List of issues that remain to be resolved |

| TODO: USE-CASE ID e.g. UC1, UC2, ... | TODO: USE-CASE NAME | 
| -------------------------------------- | ------------------- |
| **Description** | TODO: Goal to be achieved by use case and sources for requirement |
| **Actors** | TODO: List of actors involved in use case |
| **Assumptions** | TODO: Pre/post-conditions if any</td></tr>
| **Steps** | TODO: Interactions between actors and system necessary to achieve goal |
| **Variations** | TODO: OPTIONAL - Any variations in the steps of a use case |
| **Non-functional** | TODO: OPTIONAL - List of non-functional requirements that the use case must meet. |
| **Issues** | TODO: OPTIONAL - List of issues that remain to be resolved |

| TODO: USE-CASE ID e.g. UC1, UC2, ... | TODO: USE-CASE NAME | 
| -------------------------------------- | ------------------- |
| **Description** | TODO: Goal to be achieved by use case and sources for requirement |
| **Actors** | TODO: List of actors involved in use case |
| **Assumptions** | TODO: Pre/post-conditions if any</td></tr>
| **Steps** | TODO: Interactions between actors and system necessary to achieve goal |
| **Variations** | TODO: OPTIONAL - Any variations in the steps of a use case |
| **Non-functional** | TODO: OPTIONAL - List of non-functional requirements that the use case must meet. |
| **Issues** | TODO: OPTIONAL - List of issues that remain to be resolved |


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
