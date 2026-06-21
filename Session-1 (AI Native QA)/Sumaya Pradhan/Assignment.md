**Naming Conventions:**
TC_PAGENAME--- Manually written test cases.
AI_TC_PAGENAME--- Missed by me, caught by AI.

**Test cases for Welcome Page**
TC_WelcomePage_001	
Validating successful navigation to Welcome page.	
Navigate to 'https://blazedemo.com/'
		
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

_AI_TC_WelcomePage_012_
Validate system behavior when refreshing the page or using malformed URL parameters.
1.Navigate to https://blazedemo.com/.
2.Refresh the page using the browser refresh button (or press F5).
3.Observe whether the page reloads correctly and retains default dropdown values.

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

_AI_TC_ReservePage_006_
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

_AI_TC_ReservePage_007_
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
TC_PurchasePage_001	
Validating successful navigation to Purchase page.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular airline.
		
TC_PurchasePage_002	
Validating elements in Purchase page.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular airline.
		
TC_PurchasePage_003	
Validating displaying of from & to address in the header.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular airline.
		
TC_PurchasePage_004	
Validating successful update of from & to address in the header after changing it in Welcome page.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular airline.
4.Navigate back to 'Welcome Page' & update the values.
		
TC_PurchasePage_005	
Validating displaying of values for 'Airline'.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular airline.
		
TC_PurchasePage_006	
Validating successful update of 'Airline' values after changing it in Reserve page.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular airline.
4.Navigate back to 'Reserve Page' & update the values.
5.Click on the 'Choose This Fight' button.
		
TC_PurchasePage_007	
Validating  displaying of values for 'Flight Number'.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular Flight Number.
		
TC_PurchasePage_008	
Validating successful update of 'Flight Number' values after changing it in Reserve page.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular Flight Number.
4.Navigate back to 'Reserve Page' & update the values.
5.Click on the 'Choose This Fight' button.
		
TC_PurchasePage_009	
Validating  displaying of values for 'Price'.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular price.
		
TC_PurchasePage_010	
Validating successful update of 'Price' values after changing it in Reserve page.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular price.
4.Navigate back to 'Reserve Page' & update the values.
5.Click on the 'Choose This Fight' button.
		
TC_PurchasePage_011	
Validating displaying of values for 'Arbitrary Fees and Taxes'.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular price.
		
TC_PurchasePage_012	
Validating updating of values of 'Arbitrary Fees and Taxes' after changing the price.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular price.
4.Navigate back to 'Reserve Page' & update the values.
5.Click on the 'Choose This Fight' button.
		
TC_PurchasePage_013	
Validating displaying of values for 'Total Cost'.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular price.
		
TC_PurchasePage_014	
Validating 'Price'+'Arbitrary Fees & Taxes' = 'Total Cost'.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular price.
4.Calculate the total cost including 'Price' & 'Arbitrary Fees & Taxes'.
		
TC_PurchasePage_015	
Validating 'Name' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Click on the 'Name' input box.
		
TC_PurchasePage_016	
Validating placeholder for 'Name' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
		
TC_PurchasePage_017	
Validating max characters allowed in 'Name' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Click on the 'Name' input box & provide max input value.
		
TC_PurchasePage_018	
Validating min characters allowed in 'Name' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Click on the 'Name' input box & provide min input value.
		
TC_PurchasePage_019	
Validating special characters allowed in 'Name' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Click on the 'Name' input box & provide special characters.
		
TC_PurchasePage_020	Validating 'Address' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Click on the 'Address' input box.
		
TC_PurchasePage_021	
Validating placeholder for 'Address' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
		
TC_PurchasePage_022	
Validating max characters allowed in 'Address' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Click on the 'Address' input box & provide max input value.
		
TC_PurchasePage_023	
Validating min characters allowed in 'Address' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Click on the 'Address' input box & provide min input value.
		
TC_PurchasePage_024	
Validating special characters allowed in 'Address' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Click on the 'Address' input box & provide special characters.
		
TC_PurchasePage_025	
Validating 'City' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Click on the 'City' input box.
		
TC_PurchasePage_026	
Validating placeholder for 'City' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
		
TC_PurchasePage_027	
Validating max characters allowed in 'City' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Click on the 'City' input box & provide max input value.
		
TC_PurchasePage_028	
Validating min characters allowed in 'City' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Click on the 'City' input box & provide min input value.
		
TC_PurchasePage_029	
Validating special characters allowed in 'City' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Click on the 'City' input box & provide special characters.
		
TC_PurchasePage_030	
Validating 'State' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Click on the 'State' input box.
		
TC_PurchasePage_031	
Validating placeholder for 'State' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
		
TC_PurchasePage_032	
Validating max characters allowed in 'State' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Click on the 'State' input box & provide max input value.
		
TC_PurchasePage_033	
Validating min characters allowed in 'State' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Click on the 'State' input box & provide min input value.
		
TC_PurchasePage_034	
Validating special characters allowed in 'State' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Click on the 'State' input box & provide special characters.
		
TC_PurchasePage_035	
Validating 'Zip Code' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Click on the 'Zip Code' input box.
		
TC_PurchasePage_036	
Validating placeholder for 'Zip Code' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
		
TC_PurchasePage_037	
Validating max characters allowed in 'Zip Code' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Click on the 'Zip Code' input box & provide max input value.
		
TC_PurchasePage_038	
Validating min characters allowed in 'Zip Code' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Click on the 'Zip Code' input box & provide min input value.
		
TC_PurchasePage_039	
Validating special characters allowed in 'Zip Code' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Click on the 'Zip Code' input box & provide special characters.
		
TC_PurchasePage_040	
Validating 'Card Type' dropdown box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Click on the 'Card Type' dropdown value & chose a value.
		
TC_PurchasePage_041	
Validating default value for 'Card Type' dropdown box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
		
TC_PurchasePage_042	
Validating 'Credit Card Number' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Click on the 'Credit Card Number' input box.
		
TC_PurchasePage_043
Validating placeholder for 'Credit Card Number' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
		
TC_PurchasePage_044	
Validating max characters allowed in 'Credit Card Number' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Click on the 'Credit Card Number' input box & provide max input value.
		
TC_PurchasePage_045	
Validating min characters allowed in 'Credit Card Number' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Click on the 'Credit Card Number' input box & provide min input value.
		
TC_PurchasePage_046	
Validating special characters allowed in 'Credit Card Number' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Click on the 'Credit Card Number' input box & provide special characters.
		
TC_PurchasePage_047	
Validating 'Month' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Click on the 'Month' input box.
		
TC_PurchasePage_048	
Validating placeholder for 'Month' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Month' button for particular record.
		
TC_PurchasePage_049	
Validating max characters allowed in 'Month' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Click on the 'Month' input box & provide max input value.
		
TC_PurchasePage_050	
Validating min characters allowed in 'Month' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Click on the 'Month' input box & provide min input value.
		
TC_PurchasePage_051	
Validating special characters allowed in 'Month' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Click on the 'Month' input box & provide special characters.
		
TC_PurchasePage_052	
Validating 'Year' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Click on the 'Year' input box.
		
TC_PurchasePage_053	
Validating placeholder for 'Year' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Year' button for particular record.
		
TC_PurchasePage_054	
Validating max characters allowed in 'Year' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Click on the 'Year' input box & provide max input value.
		
TC_PurchasePage_055	
Validating min characters allowed in 'Year' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Click on the 'Year' input box & provide min input value.
		
TC_PurchasePage_056	
Validating special characters allowed in 'Year' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Click on the 'Year' input box & provide special characters.
		
TC_PurchasePage_057	
Validating 'Name on Card' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Click on the 'Name on Card' input box.
		
TC_PurchasePage_058	
Validating placeholder for 'Name on Card' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Name on Card' button for particular record.
		
TC_PurchasePage_059	
Validating max characters allowed in 'Name on Card' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Click on the 'Name on Card' input box & provide max input value.
		
TC_PurchasePage_060	
Validating min characters allowed in 'Name on Card' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Click on the 'Name on Card' input box & provide min input value.
		
TC_PurchasePage_061	
Validating special characters allowed in 'Name on Card' input box.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Click on the 'Name on Card' input box & provide special characters.
		
TC_PurchasePage_062	
Validating 'Purchase Flight' button.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & click on the 'Purchase Flight' button.
		
TC_PurchasePage_063	
Checking the functionality of 'Purchase Flight' button with all valid input values.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & click on the 'Purchase Flight' button.
		
TC_PurchasePage_064	
Checking the functionality of 'Purchase Flight' button with invalid input values in 'Name'.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & provide an invalid input in 'Name'.
5.Click on the 'Purchase Flight' button.
		
TC_PurchasePage_065	
Validating if 'Name' input values mandatory.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & leave the 'Name' input value blank.
5.Click on the 'Purchase Flight' button.
		
TC_PurchasePage_066	
Checking the functionality of 'Purchase Flight' button with invalid input values in 'Address'.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & provide an invalid input in 'Address'.
5.Click on the 'Purchase Flight' button.
		
TC_PurchasePage_067	
Validating if 'Address' input values mandatory.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & leave the 'Address' input value blank.
5.Click on the 'Purchase Flight' button.
		
TC_PurchasePage_068	
Checking the functionality of 'Purchase Flight' button with invalid input values in 'City'.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & provide an invalid input in 'City'.
5.Click on the 'Purchase Flight' button.
		
TC_PurchasePage_069	
Validating if 'City' input values mandatory.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & leave the 'City' input value blank.
5.Click on the 'Purchase Flight' button.
		
TC_PurchasePage_070	
Checking the functionality of 'Purchase Flight' button with invalid input values in 'State'.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & provide an invalid input in 'State'.
5.Click on the 'Purchase Flight' button.
		
TC_PurchasePage_071	
Validating if 'State' input values mandatory.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & leave the 'State' input value blank.
5.Click on the 'Purchase Flight' button.
		
TC_PurchasePage_072	
Checking the functionality of 'Purchase Flight' button with invalid input values in 'Zip Code'.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & provide an invalid input in 'Zip Code'.
5.Click on the 'Purchase Flight' button.
		
TC_PurchasePage_073	
Validating if 'Zip Code' input values mandatory.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & leave the 'Zip Code' input value blank.
5.Click on the 'Purchase Flight' button.
		
TC_PurchasePage_074	
Checking the functionality of 'Purchase Flight' button with invalid input values in 'Credit Card Number'.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & provide an invalid input in 'Credit Card Number'.
5.Click on the 'Purchase Flight' button.
		
TC_PurchasePage_075	Validating if 'Credit Card Number' input values mandatory.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & leave the 'Credit Card Number' input value blank.
5.Click on the 'Purchase Flight' button.
		
TC_PurchasePage_076	Checking the functionality of 'Purchase Flight' button with invalid input values in 'Month'.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & provide an invalid input in 'Month'.
5.Click on the 'Purchase Flight' button.
		
TC_PurchasePage_077	
Validating if 'Month' input values mandatory.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & leave the 'Month' input value blank.
5.Click on the 'Purchase Flight' button."
		
TC_PurchasePage_078	
Checking the functionality of 'Purchase Flight' button with invalid input values in 'Year'.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & provide an invalid input in 'Year'.
5.Click on the 'Purchase Flight' button.
		
TC_PurchasePage_079
Validating if 'Year' input values mandatory.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & leave the 'Year' input value blank.
5.Click on the 'Purchase Flight' button.
		
TC_PurchasePage_080	
Checking the functionality of 'Purchase Flight' button with invalid input values in 'Name on Card'.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & provide an invalid input in 'Name on Card'.
5.Click on the 'Purchase Flight' button.
		
TC_PurchasePage_081
Validating if 'Name on Card' input values mandatory.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & leave the 'Name on Card' input value blank.
5.Click on the 'Purchase Flight' button.
		
TC_PurchasePage_082	
Validating 'Remember me' checkbox.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & click on the 'Remember me' checkbox.
		
TC_PurchasePage_083	
Checking the functionality of 'Remember me' checkbox.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & click on the 'Remember me' checkbox.
5.Click on the 'Purchase Flight' button.

_AI_TC_PurchasePage_084_
Submit with all fields blank → Verify mandatory field errors.
1.Navigate to https://blazedemo.com/.
2.Select a flight and proceed to the Purchase Page.
3.Leave all input fields blank.
4.Click on the Purchase Flight button.

_AI_TC_PurchasePage_084_
Submit with extra-long inputs across multiple fields simultaneously → Ensure system handles gracefully.
1.Navigate to the Purchase Page.
2.Enter extremely long strings (e.g., 500+ characters) in multiple fields such as Name, Address, City.
3.Click on the Purchase Flight button.

_AI_TC_PurchasePage_087_ 
Validate numeric-only requirement for Zip Code.
1.Navigate to the Purchase Page.
2.Enter alphabetic or special characters in the Zip Code field.
3.Click on the Purchase Flight button.

_AI_TC_PurchasePage_088_ 
Validate numeric-only requirement for Credit Card Number.
1.Navigate to the Purchase Page.
2.Enter alphabetic or special characters in the Credit Card Number field.
3.Click on the Purchase Flight button.

_AI_TC_PurchasePage_089_ 
Validate Month accepts only 1–12.
1.Navigate to the Purchase Page.
2.Enter invalid month values (e.g., 0, 13, 99).
3.Click on the Purchase Flight button.

_AI_TC_PurchasePage_090_ 
Validate Year accepts only valid ranges (e.g., current year onward).
1.Navigate to the Purchase Page.
2.Enter past years (e.g., 2000) or unrealistic future years (e.g., 9999).
3.Click on the Purchase Flight button.

_AI_TC_PurchasePage_091_ 
Verify Credit Card Number input masks sensitive digits (e.g., shows ****).
1.Navigate to the Purchase Page.
2.Enter a valid credit card number.
3.Observe the input field while typing and after submission.

_AI_TC_PurchasePage_092_ 
Verify “Remember me” does not store sensitive payment info (only user details).
1.Navigate to the Purchase Page.
2.Fill in all details including payment info.
3.Select the Remember me checkbox.
4.Submit the form and return to the page.

_AI_TC_PurchasePage_093_ 
Validate HTTPS secure connection during purchase submission.
1.Navigate to the Purchase Page.
2.Fill in all mandatory details.
3.Click on the Purchase Flight button.

_AI_TC_PurchasePage_094_ 
Validate confirmation page shows unique booking ID/reference number.
1.Navigate to the Purchase Page.
2.Fill in all mandatory details with valid inputs.
3.Click on the Purchase Flight button.
4.On the confirmation page, check for a unique booking ID/reference number.

**Test cases for Confirmation Page**
TC_ConfirmationPage001	
Validating Successful navigation to 'Confirmation' page.
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & click on the 'Purchase Flight' button.
		
TC_ConfirmationPage002	
Validating elements in 'Thank you' page.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & click on the 'Purchase Flight' button.
		
TC_ConfirmationPage003	
Validating 'Id' value after successful purchase.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & click on the 'Purchase Flight' button.
		
TC_ConfirmationPage004	
Validating change of 'Id' value in REST API response after every successful purchase. 	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & click on the 'Purchase Flight' button.
		
TC_ConfirmationPage005	
Validating change of 'Id' value in REST API response after every failed purchase. 	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Create a failed purchase.
		
TC_ConfirmationPage006	
Validating 'Status' value after successful purchase.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & click on the 'Purchase Flight' button.
		
TC_ConfirmationPage007	
Validating 'status' value passed in REST API response after successful purchase.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & click on the 'Purchase Flight' button.
		
TC_ConfirmationPage008	
Validating 'amount' value after successful purchase.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & click on the 'Purchase Flight' button.
		
TC_ConfirmationPage009	
Validating 'amount' value passed in REST API response after successful purchase.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & click on the 'Purchase Flight' button.
		
TC_ConfirmationPage010	
Validating 'currency' value after successful purchase.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & click on the 'Purchase Flight' button.
		
TC_ConfirmationPage011	
Validating 'currency' value passed in REST API response after successful purchase.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & click on the 'Purchase Flight' button.
		
TC_ConfirmationPage012	
Validating 'currency' value after successful purchase.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & click on the 'Purchase Flight' button.
		
TC_ConfirmationPage013	
Validating 'currency' value passed in REST API response after successful purchase.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & click on the 'Purchase Flight' button.
		
TC_ConfirmationPage014	
Validating 'Card Number' value after successful purchase.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & click on the 'Purchase Flight' button.
		
TC_ConfirmationPage015	
Validating 'Card Number' value passed in REST API response after successful purchase.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & click on the 'Purchase Flight' button.
		
TC_ConfirmationPage016	
Validating 'Expiration' value after successful purchase.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & click on the 'Purchase Flight' button.
		
TC_ConfirmationPage017	
Validating 'Expiration' value passed in REST API response after successful purchase.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & click on the 'Purchase Flight' button.
		
TC_ConfirmationPage018	
Validating 'Auth Code' value after successful purchase.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & click on the 'Purchase Flight' button.
		
TC_ConfirmationPage019	
Validating 'Auth Code' value passed in REST API response after successful purchase.	
1.Navigate to 'https://blazedemo.com/'.
2.Fill all the details & click on the 'Find Flight' button.
3.Click on the 'Choose This Fight' button for particular record.
4.Fill all the mandatory details & click on the 'Purchase Flight' button.

_AI_TC_ConfirmationPage_020_
Validate “Date” value displayed on Confirmation page matches system date/time.
1.Navigate to https://blazedemo.com/.
2.Select a flight and proceed to the Purchase Page.
3.Fill all mandatory details and click Purchase Flight.
4.On the Confirmation page, note the displayed Date value.
5.Compare it with the system/browser date and time.

_AI_TC_ConfirmationPage_021_
Validate “Date” value passed in REST API response matches transaction time.
1.Complete a purchase as above.
2.Capture the REST API response for the transaction
3.Locate the Date field in the API response.
4.Compare with the system/browser transaction time.

_AI_TC_ConfirmationPage_022_
Verify only last 4 digits of card number are displayed, rest masked.
1.Complete a purchase with a valid credit card.
2.On the Confirmation page, check the Card Number field.

_AI_TC_ConfirmationPage_023_
Ensure API response does not expose full card number.
1.Complete a purchase.
2.Capture the REST API response.
3.Inspect the Card Number field.

_AI_TC_ConfirmationPage_024_
Validate presence of “self” link in API response.
1.Complete a purchase.
2.Capture the REST API response.
3.Inspect the _links section.

_AI_TC_ConfirmationPage_027_
Validate “capture” link works correctly.
1.Complete a purchase.
2.Capture the REST API response.
3.Inspect the _links section for capture.
4.Trigger the capture link via API call.

_AI_TC_ConfirmationPage_028_
Validate “reversal” link works correctly.
1.Complete a purchase.
2.Capture the REST API response.
3.Inspect the _links section for reversal.
4.Trigger the reversal link via API call.

_AI_TC_ConfirmationPage_029_
Validate behavior when API response returns error (e.g., failed capture).
1.Simulate a failed capture scenario (e.g., invalid capture request).
2.Observe the API response.

_AI_TC_ConfirmationPage_030_
Validate UI shows appropriate error message for failed purchase.
1.Attempt a purchase with invalid/malformed input to force failure.
2.Observe the Confirmation page.
