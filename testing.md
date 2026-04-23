# Testing

## Test Plan
TODO: Add rows for each test, current status is eg. pass/fail

| Use-Case ID | Requirement ID | Test Case | Status |

   **US1**        |  **FR1, FR2**      | Search by business name returns results.| **Pass** |
   **US1**        |  **FR1, FR2**      | Search by location returns results. |**Pass**|
   **US1**        |  **FR1, FR2**      | Filter by hygiene rating 5.| **Pass**|
   **UC1**        |  **FR1, FR2**      | Filter by hygiene rating 4.| **Pass**|
   **UC1**        |  **FR1, FR2**      | Filter by hygiene rating 3.| **Pass**| 
   **UC1**        |  **FR1, FR2**      | Filter by hygiene rating 2.| **Pass** |
   **UC1**        |  **FR1, FR2**      | Filter by hygiene rating 1.| **Pass**|
   **UC1**        |  **FR1, FR2**      | Filter by hygiene rating 0 (Urgent).| **Pass**| 
   **UC1**        |  **FR2**           | Display correct marker colours on map.| **Fail** |      
   **UC1**        |  **FR2**           | Display business details on marker click.| **Fail** |
    **UC2**        |  **FR4**           | Submit issue form (under map).| **Pass** |
   **UC2**        |  **FR4**           | Confirmation message appears for 3 seconds after form submission.| **Pass**| 
   **UC2**       |  **FR4**           |Full page reset after confirmation message. | **Pass** |
  **UC1**        |  **FR1, FR5**      | Reset search form clears input.| **Pass**|
   **UC1**        |  **NFR1, NFR2**    | Mobile responsiveness for dropdown.| **Pass** |
   **UC3**        |  **FR6, NFR1, NFR4** | API fallback activates if API fails. | **Pass** |
   **UC3**    |  **FR6, NFR1**       | System switches to GeoJSON backup data. |  **Pass**      |
 **UC1** | **FR3, FR4** | Toggle between Map View and List View retains search parameters.| **Pass** |
 **UC1** | **FR9** |  Searching for a nonexistent business in List View shows 'No Results Found'. | **Pass** | 
 **UC1** | **FR10,NFR9** |  Paginate through results using Next/Previous buttons. | **Pass** |
 **UC1** | **NFR12** | Verify List View scales properly on mobile. | **Pass** |
  **UC1** | **FR7** | Search by business name in List View returns correct results. | **Pass** |
 **UC1** | **FR6,FR7** | Filter by hygiene rating in List View returns correct results. | **Pass** |
 **UC1** | **FR8** | List View updates results instantly without page refresh. | **Pass** | 
| **UC1** | **FR13** | List View displays business name, address, and hygiene rating. | **Pass** |
| **UC1** | **FR14** | List View pagination displays correct number of results per page. | **Pass** |
| **UC1** | **FR15** | List View sorting by hygiene rating works correctly. | **Pass** |
| **UC1** | **FR16** | List View reset button clears all filters and search inputs. | **Pass** |



