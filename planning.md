# Project Proposal
Food Hygiene Rating Application is an app that will be designed to improve food hygiene awareness, monitoring food businesses and restaurants. The app will be both an informative and monitoring app. The application will be used by customers to solve indecisiveness when choosing a place to eat and will encourage business owners to maintain/improve their ratings due to their ratings being publically available. The app will give places that are less popular or strugging a better chance to appear so more people have the option to go there rather than leave the business near the bottom of the list.
## Business Case
Food related diseases affect millions globally each year, resulting in significant public health and economic impacts. Most people also get overwhelmed with the choices available for places to eat so this app will help customers pick quickly. The restaurants ratings will be public for the consumers to see which makes looking for a hygiene place much easier and decreases the risk of getting any illess from the business.
### Problem statement
Many food businesses/restaurants lack access to proper training and hygiene monitoring tools. Inspection systems used by health authorities are often manual, inefficient and paper-based. This makes it difficult to decide where to eat due to hygiene ratings being mostly paper-based and while online they are scattered across many different webistes making it not so easily accessible. People would want a business where they can view a place ratings and make a quick decision on where to eat.

### Business benefits
 * To help people know about hygiene ratings and encourage other restaurants to try and improve their ratings.
 * Simplifies documentation of inspections.
 * The application helps customers access information about how clean food businesses are which helps them choose safer places to eat.
 * This encourages business owners to maintain/improve their hygiene standards since their ratings will be publically available.
 * Lets hygiene inspectors look at the app and see previous reuslts and come to a place with expectations.
 * Lets more unknown restaurants be more known if they have a better hygiene rating.
 * Puts more unknown restaurants at the top so it gives exposure to more locally owned business.

### Options Considered
 Consumers can directly check offical databases such as the UK Food Standards Agency (FSA) hygiene rating site. This is quite reliable and up-to-date however, it is not convenient and isn't user friendly as an app. Restaurant reviews are often include hygiene comments or ratings from personal experiences from customers. The only potential con I can see at the moment is that from this perspective is that it is not offical ratings so can be misleading. Third party apps may show food ratings that are often inaccurate and are not regularly updated which makes them unreliable.

 ### Stakeholders
 A stakeholder is any individual, group or organisation that can affect or be affected by the actions, goals and policies of a business or project. The stakeholders of this project would be:
 - Consumers - They will try to find safe places to eat and they are the primary users of the application.
 - Business Owners - To maintain accurate ratings and their business' ratings are publically visible.
 - Food Hygiene Inspectors - To make reporting more effcient, they can view the business' old inspection results and notes.
 - Local Council/FSA - The public health enforcement, they are the data source provider for restaurants ratings.
 - Developers - They are in charge of the systems maintainence and they build/maintain the app.


### Expected Risks
The risks that may appear for the project are listed below. I have accessed what may happen and how to avoid the problems:
* Low user adoption - There is a medium likihood that users wouldn't be able to adapt to the app and this would have a high impact on the project's success. Many people already search for restaurants through competitors such as Google Maps or TripAdvisor so trying to convince users to use a dedicated food hygiene rating app will need to feel more useful rather than go to those convient apps. To avoid this, the design will include a simple User Interface to make it suitable for all age groups.
* Data/security concerns- The likihood of this is low but the impact would be high if user data was actually compromised. The app avoids this by not storing data except for people's favourite businesses. All data comes from publically available data which is uploaded from the government.
* Inaccurate or manipulated data - The risk of this inaccurate data being is low but has a high impact on the app's success. The data will come from Bristol's Open Data API dataset, there will be a small delay and updating the data but shouldn't cause delays.
* Legal challenges - The government allows public use of Bristol's dataset, this includes commerical use for business.
* Convincing users to go to less known businesses - There is a higher risk for this as people are more likely to go to more familar or popular businesses and the app's goal to try to expose less known businesses is a rather hard goal. To avoid people going to popular places, the results are placed by default rather than by popularity. If a business has excellent hygiene results than the business will have more exposure than others.


## Project Scope
The project is a food hygiene rating application that enables users to:
* Search for food businesses by name and location
* Filter businesses by hygiene rating (0-5)
* Naviagte results using next and previous buttons
* Access real life data from Bristol Open Data API with a backup data source


![Insert your Context Diagram Here](images/context.png)  Mwelwa chisesa <img width="783" height="514" alt="image" src="https://github.com/user-attachments/assets/40bcb424-d721-4626-ac45-43a56fca7639" />
The Context diagram aboves shows what we want the application to contain and the features the app will have. 

The features that the app will have are:
- Business ratings and search, this will display ratings and allow users to search for food businesses
- Government database, provides official inspection and hygiene data
- User reports, consumers can submit hygiene and safety reports
- Server system, handles bugs/fixes/updates for the application
- Server system, handles app funcitonalities and data storage for the hygiene ratings for each of the food businesses
- Consumers, search for food businesses, view ratings and report issues
- Search and filters, enables search phrases and filtering options
- Maps and GPS, guides users to food businesses using geolocation

<img width="859" height="297" alt="image" src="https://github.com/user-attachments/assets/d2ed170c-1b14-4411-88f7-e012c729a0b6" />
The Context diagram shows the features that the app will have.

These are the features that the app will contain:
- Consumers/customers will interact with the app to view food hygiene ratings for businesses which will help indecisiveness of where to eat for some people
- Search phrases, filters and favourites which allows for people to navigate the application and allows to favourite food businesses so it saves what people's favourites places to eat are
- The application needs to accommodate different types of screen sizes that allows the application to be more accessible
- Geolocation is enabled to help guide customers to different food businesses with hygiene ratings that is close to them
- Government official food database which provides official inspection results and reason for the scoring
- Displays ratings and able to search businesses by food businesses, cuisine, location or hygiene rating
- User reports which allows consumers to report any issues with food businesses
- Server infrastructure which allows memory to be used to contain reviews from customers and complaints from users
