**Naming Conventions:**
TC_PAGENAME--- Manually written test cases.
AI_TC_PAGENAME--- AI generated test cases.

**Test cases for Welcome Page**
TC_WelcomePage_001	
Validating successful navigation to Welcome page.	
Navigate to 'https://blazedemo.com/'

_AI_TC_WelcomePage_
Validate system behavior when refreshing the page or using malformed URL parameters.
1.Navigate to https://blazedemo.com/.
2.Refresh the page using the browser refresh button (or press F5).
3.Observe whether the page reloads correctly and retains default dropdown values.
		
TC_WelcomePage_002	
Validating elements in Welcome Page.	
Navigate to 'https://blazedemo.com/'
		
TC_WelcomePage_003	
Validating 'Travel The World' button in Nav bar.	
1.Navigate to 'https://blazedemo.com/'.
2.Click on the 'Travel The World' button.
		
TC_WelcomePage_004	
Validating 'home' button in Nav bar.	
1.Navigate to 'https://blazedemo.com/'.
2.Click on the 'Home' button.
		
TC_WelcomePage_005	
Validating 'Destination of the week...' link.	
1.Navigate to 'https://blazedemo.com/'.
2.Click on the 'Destination of the week...' link.
		
TC_WelcomePage_006	
Validating 'Departure City' dropdown.	
1.Navigate to 'https://blazedemo.com/'.
2.Click on the 'Departure City' dropdown.
		
TC_WelcomePage_007	
Validating 'Destination City' dropdown.	
1.Navigate to 'https://blazedemo.com/'.
2.Click on the 'Destination City' dropdown.
		
TC_WelcomePage_008	
Checking for default values in 'Departure City' & 'Destination City' dropdown.	
Navigate to 'https://blazedemo.com/'.
		
TC_WelcomePage_009	
Checkin the functionality of 'Find Flights' button.	
1.Navigate to 'https://blazedemo.com/'.
2.Click on the 'Find Flights' button.
		
TC_WelcomePage_010	
Finding valid Filghts according to 'Departure City' dropdown value.	
1.Navigate to 'https://blazedemo.com/'.
2.Click on the 'Departure City' dropdown & choose a specific dropdown value.
		
TC_WelcomePage_011	
Finding valid Filghts according to 'Destination City' dropdown value.	
1.Navigate to 'https://blazedemo.com/'.
2.Click on the 'Destination City' dropdown & choose a specific dropdown value.

**Test cases for Reserve Page**
TC_ReservePage_001	
Validating successful navigation to Reserve page.	
1.Navigate to 'https://blazedemo.com/'.
2.Set the value in 'Departure City' & 'Destination City' dropdown.
3.Click on the 'Find Flight' button.
		
TC_ReservePage_002	
Validating elements in Reserve page.	
1.Navigate to 'https://blazedemo.com/'.
2.Set the value in 'Departure City' & 'Destination City' dropdown.
3.Click on the 'Find Flight' button.
		
TC_ReservePage_003	
Validating Departs header value after updating 'Departure City'.	
1.Navigate to 'https://blazedemo.com/'.
2.Set a particular value in 'Departure City' dropdown.
3.Click on the 'Find Flight' button.
		
TC_ReservePage_004	
Validating Arrives header value after updating  'Destination City'.	
1.Navigate to 'https://blazedemo.com/'.
2.Set a particular value in 'Destination City' dropdown.
3.Click on the 'Find Flight' button.
		
TC_ReservePage_005	
Checking the functionality of 'Choose This Flight' button.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular airline.

_AI_TC_ReservePage_001_
Verify that all flights displayed match the selected Departure and Destination cities.
1.Navigate to https://blazedemo.com/.
2.Select a specific value in the Departure City dropdown (e.g., Paris).
3.Select a specific value in the Destination City dropdown (e.g., Buenos Aires).
4.Click on the Find Flights button.
5.On the Reserve Page, review the flight table:
Check the Departs column header and ensure it matches the selected Departure City.
Check the Arrives column header and ensure it matches the selected Destination City.
Verify that each flight row shows the correct departure and arrival cities consistent with the selection.
6.Repeat the test with different city combinations to confirm consistency.

_AI_TC_ReservePage_002_
Navigate directly to the Reserve page with incorrect query parameters (e.g., ?from=@@@&to=###) and check if the page handles gracefully.
1.Open the browser and navigate to the BlazeDemo Welcome Page (https://blazedemo.com/).
2.Manually enter a malformed Reserve page URL in the address bar, for example:
https://blazedemo.com/reserve.php?from=@@@&to=###
https://blazedemo.com/reserve.php?departure=invalid&destination=xyz
3.Press Enter to load the page.
Observe the behavior of the Reserve page:
Check if the page loads successfully.
Verify whether the “Departs” and “Arrives” headers show defaults or unexpected values.
Confirm whether the flight list is empty, shows incorrect data, or defaults to valid options.

**Test cases for Purchase Page**



