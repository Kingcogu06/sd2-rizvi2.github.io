# Requirements
## Functional Requirements 
The functional requirements below define what the application needs for the user's needs. Each requirement is connected to the use - case diagrams
The Functional Requirements that the food hygiene app have are:
* Search functionality -> Users are able to search for food businesses by name, hygiene rating, location or cuisine.
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
* Compatiblity -> Available and working on current IOS, Android and web platforms.
* Accessiblity -> Meet accessiblity standards.
* Screen size --> Must accommodate all screen sizes for the device that is being used.

## User Needs

#### User stories
As a **User**, I want to search for food hygiene ratings by business name, location or rating so I am able to make a good choice about where to eat.

As a **User**, I want the application to suggest nearby businesses if my search returns with no results so I can find alternatives. 

As a **User**, I want to filter search results by rating so I can identify businesses with a high standard of food hygiene.

As a **User**, I want to report any food safety issues through the application so I can alert authorities to the risks the business is accommodating.

As a **User**, I want the application to be accessible on mobile devices so that it can be used on the move. 

As a **User**, I want to recieve confirmation after submitting a report so I know my submission was successful.

As a **User**, I want the application to detect my location and for the application to show nearby businesses.

As a **User**, I want to view hygiene ratings in a list format so I can quickly scan multiple businesses without using the geolocation feature.

As a **User**, I want to naviagte through pages when there are many results so I can explore more options.

As a **User**, I want to see the total of businesses listed so I know how many options are available.

As a **Business Owner**, I want to be proud of hygiene rating as it would encourage more people to visit the business.
As a **Business Owner**, I want to be attract more customers to my business by having a high rating in food hygiene.

As a **Inspector**, I want to be able to look at old results and enter a business with expectations.

As a **Inspector**, I want to be able to decrease the amount of paper used in documenting hygiene in these businesses.

As a **Inspector**, I want to show my results publically while keeping parts of the result confidential for only the business owners to see.

As a **Developer**, I want to have access to Bristol Open Data API and implement it into the application to retrieve accurate food hygiene ratings for businesses.

### Actors
The actors and users for the food hygiene app will be:
* Users --> Consumers who want to view and search for food hygiene ratings for local food businesses/restaurants in Bristol to make decisions on where to eat and report any food related issues.
* Business Owners --> Food business owners in Bristol who want to access their information. The information that will be available on the application is the organisation's food hygiene rating, maintain their accurate information, request corrections and answer to reported incidents.
* Food Hygiene Inspector --> Inspectors come to businesses with expectations and make their reason for their grade publically which leave some things secret for only the business owner to see.
* Developer --> Responsible for creating and maintaining the database, managing corrections, handling appeals and making sure the app works properly and keeping data accurate from Bristol Open Data.

### Use Cases
| USE-CASE ID | UC1 | 
| -------------------------------------- | ------------------- |
| **Description** | Users can check food hygiene ratings, find trusted businesses.
| **Actors** | Users which can be the general public or consumers |
| **Assumptions** | <ul><li> The user knows the name, location or rating of the restaurant.</li><li> The user is familair with how to use apps and knows how to use a search feature</li><li> The user is connected to a device which can be used by Wifi or using data, the phone must be connected by a satelite signal.</li><li> The food business must have a rating for it to show up on the application.
| **Steps** | **<br>1**- User opens the web or mobile application. **<br>2**- System uses goelocation to show nearby businesses in bristol **<br>3**- User uses the search feature. **<br>4**- User enters a search term, such as Business Name, Location (Street, District or Postcode), Cuisine or Hygiene Rating. **<br>5**- User selects a rating from 0-5 to define results. **<br>6**- User clicks the 'Search' button. **<br>7**- The system sends a request to Bristol Open Data API. **<br>8**- The system displays the serach results on the map with markers for the business correlating to the results. **<br>9**- User clicks a business marker to view the organisation's details. **<br>10**- If no results are found then the system suggests nearby businesses with the same rating. **<br>11**- User clicks the 'Show list' button to switch to the list view instead of depending on the geolocation feature. **<br>12**- The system fetches the data again from Bristol Open Data API. **<br>13**- The system then displays the Business Names and Locations. **<br>14**- The system shows the number of results ( e.g. 'Showing 1-10 of 4,753 results'. **<br>15**- If there are more than 10 results, the system adds a button at the end of the page with 'Next' and 'Previous'. **<br>16**- User can control the pages using these buttons and it says at the top (e.g.Page 1-342). **<br>17**- If no results are shown, then the system displays a message that says 'No results found'. **<br>18**- The system then adds to the page suggestions with what the users picked with their filters. |
| **Variations** | <ul><li> If no results are found, the app then shows a message saying, 'No Results Found' and suggests nearby businesses. </li><li> If used filters to search then the application should suggest businesses that correlate to the users' chosen filters. </li><li> The app displays nearby businesses in Bristol </li><li> If the user enters a partial name of a business, the application matches possible matches that matches the partial input.  |
| **Non-functional** | The search should return the reuslts as quick as possible to avoid the user waiting. The app was made so that users can make quick decisions.  |
| **Issues** | The system should have a backup source in case if Bristol Open Data API has downtime for some reason and if the servers are down it should let the user know so they are prepared for slower time in getting results. |


|USE-CASE ID | UC2 | 
| -------------------------------------- | ------------------- |
| **Description** | The business owner can verify that their food hygiene rating is accurate . 
| **Actors** | Business owners and Inspectors |
| **Assumptions** | <ul><li> The business owner has access to the food hygiene application and can look at reports to their business about their ratings. </li><li> The business owner's organisation already has an existing rating in the Bristol Open Data API database so they are responsible for updating when they have a better/lower rating. </li><li> Business owners can reply to reports to say that they are working on the issue that the report has brought to light.  |
| **Steps** | **<br>1**- Business owner opens the application called GrubGrade. **<br>2**- If geolocation is allowed, the map centres on the user's location and shows nearby businesses. **<br>3**- Business owner uses the search feature. **<br>4**- Business owner enters a search term, this can be a business name or location. **<br>5**- The business owner applies a hygiene rating filter (0-5) if needed. **<br>6**- System retrieves and displays results. **<br>7**- Business owner confirms that the hygiene rating that is being displayed is accurate.**<br>8**- If incoreect the business owner fills out the correction form and submits it. **<br>9**- System confirms submission and notifies the business owner. |
| **Variations** | If the business isn't found in the application, the app then shows suggested/reccommended businesses nearby.  |
| **Non-functional** | <ul><li> The application should be available 24/7 365 days which allows consumers to report issues at anytime of the day.</li><li> The Business owners would then fix the reports as soon as posssible and can fix these anytime in the day so consumers wouldn't be confused with the inaccurate ratings. |
| **Issues** | The system must handle situations where business data is missing or outdated, this would then be fixed through the business owner to fix the inaccurate date from their end to resolve the issue. |


| USE-CASE ID | UC3 | 
| -------------------------------------- | ------------------- |
| **Description** | Food hygiene rating data can be implemented by developers via the Bristol Open Data API, with appropriate fallback and error-handling mechanisms. |
| **Actors** | Web/App developer|
| **Assumptions** | <ul><li> The developer should have access to the Bristol Open Data API and have necessary API credentials. </li><li> The API should function correctly and return data in the correct format for integration for the application.</li><li> The developer must be able to implement backup methods in case if the API fails.|
| **Steps** | **<br>1**- Developer registers for API access and gains login details. **<br>2**- The developer integrates the API data into the apllication allowing for real-time data to be displayed.**<br>3**- System then displays hygiene ratings and location on the map depending on the users filter choices or whatever is nearby if there wasn't any filter chosen.**<br>4**- If the API fails, the system then switches to a backup database, the application starts loading the data from that database and displays a message syaing that the apllication has started to use the backup data source. |
| **Variations** | If the API fails, the system starts using the backup data source and loads the backup data. |
| **Non-functional** | Fallback data should be available without any noticeable delay if the primary database fails. |
| **Issues** | If both the API and the backup data fail, then the app/web application should display an error message and askes the user to try again later. |

![Insert your Use-Case Diagram Here](images/use-case.png)
![case diagram](https://github.com/user-attachments/assets/8abffb3d-18ee-4fef-ac65-b57a7786a7b9)
The Case diagram shows all the reasons that the users can use the app for. 


Customers/Consumers can use the application for these reasons:
- To register and login
- Search for food businesses by location, cuisine, name and hygiene rating
- View hygiene ratings of restaurants
- Report hygiene problems of restaurants

Business Owners can use the application for these reasons:
- Register to manage their business
- Upload their hygiene reports so that the app can update their ratings if their ratings go down or go up.
- Responds to customers complaints and reassure them
- Be able to view inspection outcomes

Food hygiene inspectors can use the application for these reasons:
- Performs official inspections of the food businesses
- Uploads the reports to the app so that the ratings can be updated
- Assign hygiene scores

Developers can use the application for these reasons:
- Maintains the system
- Handles the bugs, fixes and updates and lag that the system may occur
- Manages the API database
  



<img width="1920" height="2560" alt="image" src="https://github.com/user-attachments/assets/b79785e1-ae18-41d8-8ea0-d9e042569ed6" />
The Case diagram aboves shows it will show how these people will interact with the app and what reasons they will use the app for.

The Food Handler will use the application for these reasons:
- Complete hygiene checklists
- Report food safety issues
- Access training guidelines
- See Inspections reports

The Manager/Supervisor will use the application for these reasons:
- Oversight of employees
- Operational management
- Food safety reports

The System admin will use the application for these reasons:
-Manage user's accounts
Manage database
Manage data updates
Keep the system updated for users to use effciently 

The Health inspector will use the application for these reasons:
- Views inspection reports
- Schedules inspections
- Manage and updates reports which leads to higher or lower hygiene ratings



## Software Requirements Specification
### Functional requirements

**FR1** - The system shall allow users to filter for food hygiene ratings using business names, locations and hygiene rating filters (1-0), UC1.

**FR2** - The system shall retrieve and display food hygiene ratings from the Bristol Open Data API database, UC1.

**FR3** - The system shall provide two views for displaying search results
* Map view --> Displays businesses as markers which users can interact with to view the businesses details.
* List view --> Displays results in a table format, including business name, location and hygiene rating.

**FR4** - The system shall allow users to switch between Map view and list view without losing some search results depending on the user's preference, UC1.

**FR5** - The system shall provide the feature of geolocation to show nearby businesses based on the user's location.
* If geolocation is enabled, the system will show a 'You are Here' marker at the user's location and display nearby locations within 500 metres of the user.
* If geolocation is denied, all businesses are displayed in a list format and doesn't involve a 'You are Here' marker, UC1.

**FR6** - The system shall allow users to use filters to help users define their search more easily. Works for both map view and list view, UC1.

**FR7** - The system shall provide a business Name and location search tool at the top of the page to allow users to filter their results, UC1.

**FR8** - The system shall update search results in real-time on the user putting partial search terms without needing a page refresh, UC1.

**FR9** - If no results are found then the system:
* Map view --> Suggests nearby businesses within the user's location if geolocation is enabled.
* List view --> Display 'No results found' at the top of the results table, UC1.

**FR10** - The system shall allow users to navigate multiple pages of results using Next and Previous buttons when many results load in, UC1.

**FR11** - The system shall display the number of results at the top of the list view, UC1.    

**FR12** - The system shall ensure that the List view is not interactive, it only shows the hygiene rating and a few details about the business such as name and hygiene rating, UC1.

**FR13** - The system shall allow food business owners to search for their food hygiene rating by name or location, UC2.

**FR14** - The system shall let users report food hygiene issues to business owners which gives them the permission to fix their food hygiene rating through a form, UC2.

**FR15** - The system shall have a report a problem form for users to use, UC2.

**FR16** - The system shall allow web developers to integrate and test the Bristol Open Data API database to ensure correct data is displayed, UC3.


### Non-Functional Requirements

**NFR1** - The system shall be available 24/7 and 365 days a year. This all0ws users and business owners to access food hygiene ratings at any time. This is significant as it allows some business owners to verify or to respond to reports outside of their business hours. If the primary Bristol Open Data database is unavailable then the system shall automatically switch to the GeoJSON backup data within a quick time ensuring that the app is always able to run, UC2.

**NFR2** - The system shall update search results and apply filters without needing a full page refresh. Search results should be appearing within 3 seconds of users submitting their filters. If the API is taking longer than 3 seconds then there shall be a visible loading indicator so that the user is aware that the system is processing their request, UC1.

**NFR3** - Switching between Map view and List view shall be seamless and keep the same results no matter the view of the results. The users should not need to reapply their search term or reapply filters when toggling between perspectives. Both perspectives must display the same businesses in the same order, UC1.

**NFR4** - The system shall inform users when the Bristol Open Data API is unavailable or having errors. This shall be displayed an alert message at the top of the results which tells the user that the main data API is unavaiable and the system has now started to use the backup database. The message shan't be too overwhelming for the user and not too technical so that the users can undertsand it clearly, UC1, UC3.

**NFR5** - The system shall display an error message if the Bristol Open Data API fails and use a GeoJSON for data retrieval. Displays a message when the first database fails and informs the user that the system started using the backup database. If both databases are down then the website will then display message that states to 'Try again later', UC1, UC3.

**NFR6** - Page navigation should be responsive and efficient. When a user clicks next or previous then the results should load without needing a full refresh. the current page number and total result count shall always be visible to the user. The naviagtion controls shall always remian visible for all screen sizes and shouldn't be hidden on mobile devices due to their decreased screen sizes, UC1.

**NFR7** - The system shall be able to handle large datasets effectively. The system should be able to search, filter and naviagte through pages without any latency. Results should be loaded in pages of 10 results at a time so there is not too much overwhelming the browser with too much data at once and confusing the user. , UC1.

**NFR8** - The report a problem form should be accessible for all users. The form should have clear labels for each field and placeholder text explaining what information is needed in each section. There should be a message after completing the report to let the users know that their submission has been confirmed, UC1, UC2.

**NFR9** - The website shall be fully functional across all screen types. The layout shall have responsiveness CSS. The application shall meet basic accessiblity standards for the application to be accessible to more users, UC1.


