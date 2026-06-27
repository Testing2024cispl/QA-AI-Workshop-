QA Manual Test Cases:------------------------------------------------------------------------------------

Module - Filter And Sorting functionality.

TC_CAT_001	Verify the category page loads successfully	
1. Open the Grocery Store website.
2. Navigate to Chocolates & Candies category.
3. Verify the category page loads without any error.
4. Verify category name and item count are displayed.
                     				
TC_CAT_002	Verify all products are displayed on the category page	
1. Open the Chocolates & Candies page.
2. Scroll through the product listing.
3. Verify each product displays image, name, price, and ADD button.
4. Ensure no product card is broken.
                     				
TC_CAT_003	Verify user can filter products using a single price range	
1. Open the category page.
2. Click the ₹0 - ₹40 price filter checkbox.
3. Verify only products within that price range are displayed.
4. Verify unrelated products are removed from the listing.
                      				
TC_CAT_004	Verify multiple price filters can be selected together	
1. Open the category page.
2. Select ₹0 - ₹40 and ₹40 - ₹80 filters.
3. Verify products from both selected ranges are displayed.
4. Verify no products outside these ranges are shown.
5. 																							
TC_CAT_005	Verify the "Clear all" option resets applied filters	
1. Apply one or more price filters.
2. Click Clear all.
3. Verify all checkboxes become unchecked.
4. Verify the complete product list is displayed again.
                   				
TC_CAT_006	Verify Featured sorting is applied by default
1. Open the category page.
2. Observe the Sort by dropdown.
3. Verify Featured is selected by default.
4. Verify products are displayed in featured order.
                      				
TC_CAT_007	Verify sorting by Discount works correctly	
1. Open the Sort by dropdown.
2. Select Discount.
3. Verify products refresh.
4. Verify products with higher discounts appear before lower discount products.																							
TC_CAT_008	Verify sorting by Price Low to High
1. Open the Sort by dropdown.
2. Select Price low to high.
3. Verify product prices are displayed in ascending order.
4. Scroll through the list to confirm sorting consistency.
                      				
TC_CAT_009	Verify sorting by Price High to Low	
1. Open the Sort by dropdown.
2. Select Price high to low.
3. Verify products are arranged from highest price to lowest price.
4. Ensure sorting remains correct after scrolling.
                      				
TC_CAT_010	Verify the selected sort option remains active after page refresh	
1. Select Price low to high.
2. Refresh the page.
3. Verify whether the selected sort option is retained or reset as per expected behavior.
4. Verify products match the selected sorting.
                      				
TC_CAT_011	Verify clicking the ADD button adds the product to the cart	
1. Open the category page.
2. Click the ADD button for any product.
3. Verify the product is added to the cart.
4. Verify the cart count is updated.
                      				
TC_CAT_012	Verify product details remain unchanged after applying filters and sorting	
1. Note the product name and price.
2. Apply a filter and sorting option.
3. Locate the same product.
4. Verify its name, image, and price remain unchanged.
                      				
TC_CAT_013	Verify browser URL remains correct after applying sorting and filters	
1. Open the category page.
2. Apply a price filter.
3. Select a sorting option.
4. Verify the URL is valid and the page does not navigate to an incorrect category or error page.																							
TC_CAT_014	Verify user can combine filtering and sorting together	
1. Select the ₹0 - ₹40 price filter.
2. Choose Price low to high sorting.
3. Verify only filtered products are displayed.
4. Verify those filtered products are sorted in ascending price order.																							
TC_CAT_015	Verify page behavior when no products match the selected filter
1. Apply a price filter that has no matching products (if available).
2. Verify an appropriate No products found message is displayed.
3. Verify the page does not break.
4. Click Clear all and verify products are displayed again.

Prompt used for AI Test case Generation -------------------------------------------------------------------

1. QA Test Case Generation Prompt - Product Filter & Listing Page
Act as a Senior QA Engineer in Manual and Automation Testing.


Analyze the attached Product Category Listing page and generate comprehensive test cases for the Product Filter and Product Listing functionality.

Create the test cases in a professional table with:
1. Test Case ID
2. Module
3. Test Scenario
4. Test Case Description
5. Preconditions
6. Test Steps
7. Test Data
8. Expected Result
9. Priority
10. Severity
11. Test Type

Generate test cases only for:

1. FILTER FUNCTIONALITY
- Price filter display
- Single and multiple filter selection
- Checkbox selection/deselection
- Filter result validation
- Product count update
- Clear All
- Refresh behavior
- Browser back/forward
- No product scenario
- Rapid clicks
- Slow network
- Invalid/empty API response
- Filter API validation
- Positive, negative, boundary and edge cases

2. SORT FUNCTIONALITY
- Featured
- Discount
- Price Low to High
- Price High to Low
- Sort after filter
- Sort after refresh
- Duplicate prices
- Rapid sort switching
- Invalid/empty API response

3. PRODUCT CARD UI TESTING
- Product image
- Broken image
- Product name
- Product price
- Currency format
- Card alignment
- Grid alignment
- Responsive grid layout
- Hover effect
- Duplicate products
- Missing product Handelling

4. RESPONSIVE TESTING
- Desktop
- Tablet
- Android
- iPhone
- Portrait/Landscape
- Small/Large resolutions

5. COMPATIBILITY TESTING
- Chrome
- Firefox
- Edge
- Safari

6. USABILITY TESTING
- Filter usability
- Sort usability
- Keyboard navigation


8. PERFORMANCE TESTING
- Filter response time
- Sort response time
- Page load time
- Slow network

9. LOAD TESTING
- 100 users
- 500 users

10. END-TO-END TESTING
- Complete user journey.

11. MONKEY TESTING
- Random clicks
- Random filters
- Random sorting

12. GORILLA TESTING
- Repeated filter apply/remove
- Repeated sorting
- Repeated refresh

Output Requirement:
Generate 50 professional test cases including positive, negative, boundary and edge cases, suitable for Excel and docs.
   

AI Manual Test Cases -----------------------------------------------------------------------------------

 TC_F01 Verify price filter section is visible on the category listing page

1. Navigate to the category listing page.
2. Locate the Filter panel on the left or top of the page.
3. Verify the Price Filter section is displayed.
4. Verify all available price range options are visible.

TC_F02 Verify user can select a single price range filter

1. Navigate to the category listing page.
2. Select the **$0–$50** price range checkbox.
3. Verify the selected checkbox is checked.
4. Verify only products within the **$0–$50** price range are displayed.

TC_F03 Verify user can select multiple price range filters simultaneously

1. Navigate to the category listing page.
2. Select the **$0–$50** price range checkbox.
3. Select the **$50–$100** price range checkbox.
4. Verify both checkboxes remain selected.
5. Verify products from both selected price ranges are displayed.

TC_F04 Verify deselecting a filter removes its effect

1. Apply the **$0–$50** price filter.
2. Click the same checkbox again to deselect it.
3. Verify the checkbox becomes unchecked.
4. Verify the product listing returns to its original state.

TC_F05 Verify all displayed products belong to the selected price range

1. Navigate to the category listing page.
2. Apply the **$50–$100** price filter.
3. Verify every displayed product price falls within the selected range.
4. Verify no products outside the selected price range are displayed.

 TC_F06 Verify product count updates after applying a filter

1. Note the initial product count.
2. Apply the **$0–$50** price filter.
3. Verify the product count updates.
4. Verify the updated count matches the displayed products.
 TC_F07 Verify the "Clear All" option removes all applied filters

1. Apply one or more price filters.
2. Click the **Clear All** button.
3. Verify all selected checkboxes become unchecked.
4. Verify all filters are removed.
5. Verify the complete product list is displayed again.
6. Verify the product count resets.

 TC_F08 Verify filter behavior after page refresh

1. Apply the **$50–$100** price filter.
2. Refresh the browser page.
3. Verify whether the applied filter persists or resets according to the business requirement.
4. Verify the behavior is consistent after every refresh.

 TC_F09 Verify behavior when no products match the selected filter

1. Navigate to the category listing page.
2. Apply a price filter with no matching products (for example **$500–$1000**).
3. Verify the product grid becomes empty.
4. Verify a **"No Products Found"** message is displayed.
5. Verify the product count displays **0**.

 TC_F10 Verify application stability during rapid filter selection

1. Navigate to the category listing page.
2. Rapidly click the same price filter checkbox multiple times.
3. Verify the application does not freeze or crash.
4. Verify no duplicate requests occur.
5. Verify the final filter state is correct.

 TC_F11 Verify filter functionality on a slow network

1. Open Developer Tools.
2. Set the network speed to **Slow 3G**.
3. Navigate to the category listing page.
4. Apply a price filter.
5. Verify a loading spinner or skeleton loader appears.
6. Verify products load successfully without errors.

 TC_F12 Verify displayed products match the filter API response

1. Open the browser Developer Tools.
2. Navigate to the **Network** tab.
3. Apply the **$50–$100** price filter.
4. Capture the API response.
5. Compare the API response with the displayed products.
6. Verify both datasets match exactly.

 TC_F13 Verify filter state after browser Back navigation

1. Apply the **$0–$50** price filter.
2. Open any product details page.
3. Click the browser **Back** button.
4. Verify the previously applied filter remains selected.
5. Verify the filtered product list is restored correctly.

 TC_F14 Verify filter panel accessibility after browser resize

1. Apply any price filter.
2. Resize the browser window from full screen to half width.
3. Verify the filter panel remains accessible or collapses into a menu.
4. Verify the applied filters remain selected.
5. Verify the filtered product list remains unchanged.

TC_S01 Verify "Featured" sort option displays products in featured order

1. Navigate to the category listing page.
2. Click the **Sort** dropdown.
3. Select the **Featured** option.
4. Verify products are displayed in the predefined featured order.
5. Verify no random ordering is observed.

 TC_S02 Verify products are sorted in ascending price order

1. Navigate to the category listing page.
2. Click the **Sort** dropdown.
3. Select **Price: Low to High**.
4. Verify the products are displayed from the lowest price to the highest price.
5. Verify the sorting order is correct for all displayed products.

 TC_S03 Verify products are sorted in descending price order

1. Navigate to the category listing page.
2. Click the **Sort** dropdown.
3. Select **Price: High to Low**.
4. Verify the products are displayed from the highest price to the lowest price.
5. Verify the sorting order is correct for all displayed products.

 TC_S04 Verify products are sorted by highest discount

1. Navigate to the category listing page containing discounted products.
2. Click the **Sort** dropdown.
3. Select the **Discount** option.
4. Verify products with the highest discount percentage appear first.
5. Verify the remaining products are displayed in descending discount order.

 TC_S05 Verify sorting works correctly after applying a filter

1. Navigate to the category listing page.
2. Apply the **$0–$100** price filter.
3. Click the **Sort** dropdown.
4. Select **Price: Low to High**.
5. Verify only filtered products are displayed.
6. Verify the filtered products are sorted in ascending price order.

 TC_S06 Verify stable sorting when products have identical prices

1. Navigate to the category listing page.
2. Select **Price: Low to High** sorting.
3. Identify products having identical prices.
4. Verify products with the same price maintain a consistent secondary order.
5. Verify the order remains consistent after refreshing the page.

 TC_S07 Verify sort behavior after page refresh

1. Navigate to the category listing page.
2. Select **Price: High to Low** from the Sort dropdown.
3. Refresh the browser page.
4. Verify the selected sorting option persists or resets according to the business requirement.
5. Verify the behavior remains consistent.

 TC_S08 Verify application stability during rapid sort switching

1. Navigate to the category listing page.
2. Quickly switch between all available sort options multiple times.
3. Verify the application remains responsive.
4. Verify no duplicate products are displayed.
5. Verify the final selected sorting option is applied correctly.

TC_S09 Verify graceful handling when no product data is returned

1. Load the category listing page with an empty product response.
2. Click the **Sort** dropdown.
3. Select any available sorting option.
4. Verify the application does not crash.
5. Verify a **"No Products Available"** message is displayed.
6. Verify the Sort dropdown remains functional.

TC_UI01 Verify product images are visible on all product cards

1. Navigate to the category listing page.
2. Observe all product cards displayed on the page.
3. Verify each product card displays a product image.
4. Verify the images are clear and properly aligned.

 TC_UI02 Verify fallback image is displayed for broken product images

1. Navigate to the category listing page containing a product with an invalid image URL.
2. Locate the affected product card.
3. Verify the broken image icon is not displayed.
4. Verify a placeholder or fallback image is displayed instead.

 TC_UI03 Verify product names are displayed correctly

1. Navigate to the category listing page.
2. Observe the product name on each product card.
3. Verify every product name is visible.
4. Verify long product names are truncated with an ellipsis.
5. Verify the text does not overflow outside the product card.

TC_UI04 Verify product prices are displayed correctly

1. Navigate to the category listing page.
2. Observe the price displayed on each product card.
3. Verify every product displays a valid price.
4. Verify the price format is correct.

TC_UI05 Verify currency symbol and price format

1. Navigate to the category listing page.
2. Observe the pricing information for multiple products.
3. Verify the correct currency symbol is displayed.
4. Verify prices contain two decimal places.
5. Verify the formatting follows the expected locale.
 TC_UI06 Verify product cards are aligned properly in the grid

1. Navigate to the category listing page.
2. Observe the product grid layout.
3. Verify all product cards are aligned uniformly.
4. Verify there are no overlapping or misaligned cards.

TC_UI07 Verify all product cards maintain equal height

1. Navigate to the category listing page.
2. Compare product cards with short and long product names.
3. Verify all cards within the same row have equal height.
4. Verify the layout remains consistent across the grid.

TC_UI08 Verify hover effect on product cards

1. Navigate to the category listing page using a desktop browser.
2. Hover the mouse over a product card.
3. Verify the configured hover effect is displayed.
4. Verify the hover effect is smooth and visually consistent.

TC_UI09 Verify no duplicate products appear in the listing

1. Navigate to the category listing page.
2. Scroll through the complete product list.
3. Compare product names or IDs.
4. Verify each product appears only once.
5. Verify no duplicate product cards are displayed.

TC_UI10 Verify handling of incomplete product information

1. Navigate to the category listing page containing a product with incomplete information.
2. Locate the affected product card.
3. Verify the product card renders successfully.
4. Verify missing information is replaced with placeholders or hidden gracefully.
5. Verify the page layout remains unaffected.

TC_UI11 Verify responsive product grid layout

1. Open the category listing page on a desktop screen.
2. Verify the product grid displays four columns.
3. Resize the browser to tablet resolution.
4. Verify the product grid adjusts to two columns.
5. Resize the browser to mobile resolution.
6. Verify the product grid adjusts to a single column.
7. Verify there is no horizontal scrolling or broken layout.

TC_R01 Verify page layout on desktop screen

1. Open the category listing page on a desktop browser with **1920×1080** resolution.
2. Verify the filter panel is visible on the left side.
3. Verify the sort option is displayed at the top.
4. Verify the product grid displays correctly.
5. Verify there is no UI overflow or broken layout.

TC_R02 Verify page layout on tablet screen

1. Open the category listing page on a tablet device or emulator with **768×1024** resolution.
2. Verify the filter panel collapses into a drawer or toggle.
3. Verify the product grid displays two columns.
4. Verify all text and UI elements are readable.
5. Verify there are no layout issues.

TC_R03 Verify page layout on Android mobile device

1. Open the category listing page on an Android device.
2. Verify the product grid displays a single column.
3. Verify the filter is accessible through a drawer or button.
4. Verify there is no horizontal scrolling.
5. Verify all UI elements are properly aligned.

TC_R04 Verify page layout on iPhone Safari

1. Open the category listing page on an iPhone using Safari.
2. Verify the page loads successfully.
3. Verify all content is visible without clipping.
4. Verify touch targets are easily accessible.
5. Verify the layout is responsive and user-friendly.

TC_R05 Verify layout adapts correctly on device rotation

1. Open the category listing page on a mobile device.
2. View the page in portrait mode.
3. Rotate the device to landscape mode.
4. Verify the layout adjusts correctly.
5. Rotate back to portrait mode.
6. Verify no UI elements are broken or misplaced.

TC_C01 Verify functionality on Google Chrome browser

1. Open the category listing page in the latest version of Google Chrome.
2. Apply a filter.
3. Change the sorting option.
4. Verify products are displayed correctly.
5. Verify all features function without errors.

TC_C02 Verify functionality on Mozilla Firefox browser

1. Open the category listing page in the latest version of Mozilla Firefox.
2. Apply a filter.
3. Change the sorting option.
4. Verify products load correctly.
5. Verify all functionalities work as expected.

TC_C03 Verify functionality on Safari browser

1. Open the category listing page in Safari.
2. Apply a filter.
3. Change the sorting option.
4. Verify products are displayed correctly.
5. Verify there are no browser-specific UI issues.

 TC_C04 Verify functionality on Microsoft Edge browser

1. Open the category listing page in Microsoft Edge.
2. Apply a filter.
3. Change the sorting option.
4. Verify the product listing updates correctly.
5. Verify there are no layout or functionality issues.

TC_U01 Verify filters can be accessed using keyboard navigation

1. Open the category listing page.
2. Use the **Tab** key to navigate to the filter section.
3. Use **Space** or **Enter** to select a filter.
4. Verify the filter is applied successfully.
5. Verify the focus indicator remains visible.

TC_U02 Verify filter labels are clear and understandable

1. Open the category listing page.
2. Review all available filter labels.
3. Verify each label clearly describes its purpose.
4. Verify there are no spelling mistakes or truncated labels.
5. Verify the labels are easy for users to understand.

TC_U03 Verify sort dropdown supports keyboard accessibility

1. Open the category listing page.
2. Use the **Tab** key to focus on the Sort dropdown.
3. Press **Enter** or **Space** to open it.
4. Navigate the options using the arrow keys.
5. Select an option using **Enter**.
6. Verify the selected sorting option is applied successfully.

TC_P01 Verify category page loads within the acceptable time

1. Clear the browser cache.
2. Navigate to the category listing page.
3. Measure the page load time.
4. Verify the page becomes fully interactive within the expected time.
5. Verify there are no loading or rendering issues.

TC_P02 Verify filter response time after selection

1. Open the category listing page.
2. Apply the **$0–$50** price filter.
3. Measure the time taken for the product list to refresh.
4. Verify the filtered products are displayed promptly.
5. Verify the response time is within the acceptable limit.

TC_P03 Verify page usability on a Slow 3G network

1. Open Developer Tools.
2. Throttle the network to **Slow 3G**.
3. Navigate to the category listing page.
4. Apply a price filter.
5. Change the sorting option.
6. Verify a loading indicator is displayed.
7. Verify the page loads successfully without crashing.

TC_E01 Verify the complete user journey from filter to sorting

1. Open the category listing page.
2. Verify products are displayed successfully.
3. Apply the **$0–$50** price filter.
4. Verify only filtered products are displayed.
5. Select **Price: Low to High** from the Sort dropdown.
6. Verify the filtered products are sorted correctly.
7. Click **Clear All**.
8. Verify all filters are removed.
9. Refresh the page.
10. Verify the product listing loads successfully without errors.

TC_L01 Verify system performance with 100 concurrent users

1. Configure the load testing tool for **100 concurrent users**.
2. Execute the load test against the category listing page.
3. Monitor response time and server performance.
4. Verify all users can access the page successfully.
5. Verify the error rate remains within the acceptable threshold.

 TC_L02 Verify system performance with 500 concurrent users

1. Configure the load testing tool for **500 concurrent users**.
2. Gradually increase the user load over five minutes.
3. Monitor server response time and resource utilization.
4. Verify the application remains stable.
5. Verify no server errors or performance degradation occur beyond the acceptable limit.

TC_M01 Verify application stability during random user actions

1. Open the category listing page.
2. Randomly select and deselect different filters.
3. Randomly change sorting options.
4. Scroll the page continuously.
5. Resize the browser window repeatedly.
6. Continue random actions for several minutes.
7. Verify the application does not crash or freeze.
8. Verify the UI remains functional throughout the test.

 TC_G01 Verify application stability during repetitive filter operations

1. Open the category listing page.
2. Apply the **$0–$50** price filter.
3. Click **Clear All**.
4. Repeat the apply and clear process for **50 consecutive cycles**.
5. Monitor application performance during execution.
6. Verify there are no crashes or memory leaks.
7. Verify the UI remains consistent after all iterations.
8. Verify the filter functionality continues to work correctly.


=====================================Session - 2 (Skill.MD)===============================================
URL - https://grocerystoredemo.pcubeweb.com/

Skill Used for writting the test cases by AI --------------------------------------------------------
==========================
# Purpose of Test Cases
==========================
The purpose of these test cases is to verify the functionality, usability, performance, and overall quality of the **Product Category Listing (PLP)** page in an eCommerce application.

These test cases are designed to ensure that users can efficiently browse, filter, sort, and view products while the application behaves consistently across different browsers, devices, screen resolutions, and network conditions.

The test suite validates that:

* Product filters are displayed correctly and function as expected.
* Users can apply, remove, and combine filters without affecting application stability.
* Sorting options display products in the correct order according to business rules.
* Product cards display accurate information, including images, names, prices, and currency formatting.
* Product count is updated correctly after filtering and sorting operations.
* The application behaves correctly after page refresh and browser navigation (Back/Forward).
* API responses are accurately reflected in the user interface.
* Responsive layouts adapt properly across desktop, tablet, and mobile devices.
* The application provides a consistent experience across supported browsers and operating systems.
* The Product Listing page performs efficiently under normal and slow network conditions.
* The application remains stable under concurrent user load and repeated user interactions.
* End-to-end user journeys execute successfully without data loss or functional failures.
* Random (Monkey) and repetitive (Gorilla) testing confirm the application's robustness and long-term stability.
* Business rules, data integrity, usability, and accessibility requirements are satisfied throughout the Product Listing workflow.

Overall, these test cases aim to identify functional defects, UI inconsistencies, performance bottlenecks, and business logic issues before release, ensuring a reliable, high-quality, and user-friendly shopping experience for end users.

QA Test Case Generation Prompt – Product Filter & Listing Page
================================
1. Role – Define Expertise Level
================================
Act as a Senior QA Engineer with 5+ years of experience in both Manual and Automation Testing, specializing in eCommerce web applications.
You have expertise in:
Functional Testing
UI/UX Testing
API Validation
Responsive Testing
Cross-browser Testing
Compatibility Testing
Usability Testing
Performance Testing
Load Testing
End-to-End Testing
Monkey Testing
Gorilla Testing
Boundary Value Analysis
Negative Testing
Edge Case Testing
Regression Testing
Generate professional, reusable, and industry-standard test cases suitable for experienced QA Engineers.
=========================================
2. Context – Provide Business Information
=========================================
You are testing an eCommerce Product Category Listing (PLP) page.
The page includes the following components:
Product Listing Grid
Product Cards
Price Filter
Sorting Options
Product Count
Filter Panel
Clear All Button
The goal is to validate the Product Listing page from both business and technical perspectives, ensuring users can efficiently filter, sort, and browse products across different browsers, devices, and network conditions.
The generated test cases should be reusable for:
Excel
Microsoft Word
===============================
3. Task – Specify the Objective
===============================
Analyze the Product Category Listing page and generate 50 comprehensive QA test cases covering the following modules.
===============================
Module 1 – Filter Functionality
===============================
Generate positive, negative, boundary, and edge test cases for:
Price filter visibility
Single filter selection
Multiple filter selection
Checkbox selection and deselection
Filter result validation
Product count update
Clear All functionality
Page refresh behavior
Browser Back and Forward navigation
No product found scenario
Rapid multiple filter clicks
Slow network behavior
Invalid or empty API response
Filter API response validation
=============================
Module 2 – Sort Functionality
=============================
Generate test cases for:
Featured sorting
Discount sorting
Price: Low to High
Price: High to Low
Sorting after applying filters
Sorting after page refresh
Duplicate price handling
Rapid switching between sorting options
Invalid or empty API response
==================================
Module 3 – Product Card UI Testing
==================================
Generate UI validation test cases for:
Product image
Broken image handling
Product name
Product price
Currency format
Card alignment
Grid alignment
Responsive grid layout
Hover effects
Duplicate product display
Missing product information handling
=============================
Module 4 – Responsive Testing
=============================
Generate test cases for:
Desktop
Tablet
Android devices
iPhone devices
Portrait mode
Landscape mode
Small screen resolutions
Large screen resolutions
================================
Module 5 – Compatibility Testing
================================
Generate test cases for:
Browsers
Chrome
Firefox
Edge
Safari
Verify consistent behavior across all supported browsers.
============================
Module 6 – Usability Testing
============================
Generate test cases for:
Filter usability
Sorting usability
Keyboard navigation
Overall user experience
==============================
Module 7 – Performance Testing
==============================
Generate performance scenarios for:
Filter response time
Sorting response time
Page load time
Slow network performance
=======================
Module 8 – Load Testing
=======================
Generate load testing scenarios for:
100 concurrent users
500 concurrent users
=============================
Module 9 – End-to-End Testing
=============================
Generate complete user journey scenarios covering:
Open Product Listing page
Verify products load successfully
Apply filters
Verify filtered results
Change sorting option
Verify sorted products
Refresh page
Navigate using browser Back and Forward buttons
Verify application behavior throughout the complete workflow
==========================
Module 10 – Monkey Testing
==========================
Generate random testing scenarios for:
Random clicks
Random filter selection
Random sorting changes
Verify application stability under unpredictable user actions.
===========================
Module 11 – Gorilla Testing
===========================
Generate repetitive testing scenarios for:
Repeated filter apply/remove
Repeated sorting changes
Repeated page refresh
Verify:
Application stability
UI consistency
Recovery after prolonged usage
======================================
5. Format – Control Output Structure
======================================
Generate the test cases in a professional tabular format with the following columns:
Test Case ID
Module
Test Scenario
Test Case Description
Preconditions
Test Steps
Test Data
Expected Result
Priority
Severity
Test Type

Use sequential test case IDs such as:
TC_FIL_001
TC_SORT_001
TC_UI_001
TC_RESP_001
TC_COMP_001
TC_USAB_001
TC_PERF_001
TC_LOAD_001
TC_E2E_001
TC_MONKEY_001
TC_GORILLA_001
Ensure the output is suitable for direct import into:
Excel
Microsoft Word
==========================================
5. Constraints – Set Boundaries and Limits
==========================================
Generate exactly 50 unique test cases.
Do not create duplicate scenarios.
Include positive, negative, boundary, edge, regression, UI, API validation, and performance scenarios where applicable.
Use clear, concise, and reusable test case names.
Provide step-by-step execution steps.
Include realistic test data whenever applicable.
Ensure expected results are specific and measurable.
Assign appropriate Priority (High/Medium/Low) and Severity (Critical/Major/Minor).
Follow QA industry best practices and maintain consistent formatting.
Group test cases by module and use sequential Test Case IDs.
The final output should be professional, easy to understand, and ready for immediate use in QA documentation or test management tools.

Output ----------------------------------------------------------------------------------------

TC_FIL01 Verify Price Filter Display
-------------------------------------
Open the Product Category Listing page.
Verify the Filter panel is displayed.
Verify the Price Filter section is visible.
Verify all configured price ranges are displayed.
Verify the filter labels are readable and properly aligned.

Expected Result

The Price Filter section is displayed successfully.
All configured price ranges are visible.
Filter labels are correctly aligned and readable.
No UI issues are observed.

TC_FIL02 Verify Single Price Filter Selection
---------------------------------------------
Open the Product Category Listing page.
Select a single price range (e.g., ₹0 – ₹500).
Wait for the product list to refresh.
Verify the selected checkbox remains checked.
Verify only products within the selected price range are displayed.
Verify the product count is updated.

Expected Result

Selected filter is applied successfully.
Only products within the selected price range are displayed.
Product count is updated correctly.
No unrelated products are displayed.

TC_FIL03 Verify Multiple Price Filter Selection
-----------------------------------------------
Open the Product Category Listing page.
Select the first price range.
Select another price range.
Wait until the product list refreshes.
Verify both selected checkboxes remain checked.
Verify products from both selected price ranges are displayed.

Expected Result

Multiple filters are applied successfully.
Products matching the selected price ranges are displayed.
Product count reflects the filtered results.
No duplicate products are displayed.

TC_FIL04 Verify Checkbox Selection and Deselection
--------------------------------------------------
Open the Product Category Listing page.
Select any price filter checkbox.
Verify the checkbox is selected.
Click the same checkbox again.
Verify the checkbox is deselected.
Verify the product list returns to its previous state.

Expected Result

Checkbox selection and deselection work correctly.
Product list updates accordingly.
No UI inconsistencies are observed.

TC_FIL05 Verify Filtered Products Belong to Selected Price Range
-----------------------------------------------------------------
Open the Product Category Listing page.
Apply the ₹500 – ₹1000 price filter.
Wait for products to load.
Verify the price of each displayed product.
Compare displayed prices with the selected filter range.

Expected Result

Every displayed product belongs to the selected price range.
No product outside the selected range is displayed.
Filter accuracy is maintained.

TC_FIL06 Verify Product Count Updates After Applying Filter
-----------------------------------------------------------
Open the Product Category Listing page.
Note the initial product count.
Apply a price filter.
Wait until the products reload.
Compare the updated product count with the displayed products.

Expected Result

Product count updates immediately after applying the filter.
Displayed count matches the number of products shown.
No count mismatch is observed.

TC_FIL07 Verify Clear All Functionality
---------------------------------------
Open the Product Category Listing page.
Apply multiple price filters.
Verify the products are filtered.
Click the Clear All button.
Verify all filters are removed.
Verify the complete product list is displayed again.

Expected Result

All selected filters are removed successfully.
Product list returns to the default state.
Product count is restored.
All checkboxes become unchecked.

TC_FIL08 Verify Filter Behavior After Page Refresh
-------------------------------------------------
Open the Product Category Listing page.
Apply a price filter.
Refresh the browser.
Observe the selected filter.
Verify product listing after refresh.

Expected Result

Filter behavior matches the application requirement.
Selected filter either persists or resets correctly.
Product listing remains consistent.
No application errors occur after refresh.

TC_FIL09 Verify Filter Behavior Using Browser Back and Forward
--------------------------------------------------------------
Open the Product Category Listing page.
Apply a price filter.
Open any product detail page.
Click the browser Back button.
Verify the previously selected filter.
Click the browser Forward button.
Verify the application state.

Expected Result

Previously selected filters are restored correctly.
Product listing remains consistent.
Browser navigation does not break the filter functionality.

TC_FIL10 Verify No Product Found Scenario
-----------------------------------------
Open the Product Category Listing page.
Apply a price filter that has no matching products.
Wait for the product list to refresh.
Verify the empty state message.
Verify no products are displayed.
Remove the applied filter.

Expected Result

A "No Products Found" message is displayed.
Product grid is empty.
Application remains stable.
Removing the filter restores the product list.

TC_FIL11 Verify Filter Behavior During Rapid Multiple Clicks
------------------------------------------------------------
Open the Product Category Listing page.
Click the same Price Filter checkbox repeatedly (10–15 times).
Quickly select and deselect multiple price filters.
Observe the product listing while filters are being applied.
Verify the final selected filter state.

Expected Result

The application remains responsive.
No duplicate filter requests occur.
The final selected filters are applied correctly.
No UI freezing or unexpected behavior is observed.

TC_FIL12 Verify Filter Functionality on Slow Network
----------------------------------------------------
Open the browser Developer Tools.
Throttle the network to Slow 3G.
Open the Product Category Listing page.
Apply a price filter.
Observe the loading indicator.
Verify the filtered products after loading completes.

Expected Result

A loading indicator is displayed while data is loading.
Products load successfully after the response is received.
No application crash or timeout occurs.
Filter results are displayed correctly.

TC_FIL13 Verify Filter API Response Matches Displayed Products
--------------------------------------------------------------
Open the Product Category Listing page.
Open the browser Network tab.
Apply a price filter.
Capture the filter API response.
Compare the API response with the displayed products.
Verify product count and product details.

Expected Result

Products displayed on the UI exactly match the API response.
Product count matches the API response.
No missing or extra products are displayed.

TC_FIL14 Verify Invalid Filter API Response Handling
-----------------------------------------------------
Configure the filter API to return an invalid response.
Open the Product Category Listing page.
Apply any price filter.
Observe the application behavior.
Verify the error handling.

Expected Result

The application handles the invalid response gracefully.
A user-friendly error message is displayed.
No broken UI or application crash occurs.

TC_FIL15 Verify Empty Filter API Response Handling
---------------------------------------------------
Configure the filter API to return an empty product list.
Open the Product Category Listing page.
Apply a price filter.
Wait for the response.
Observe the product listing.

Expected Result

A "No Products Found" message is displayed.
Product grid remains empty.
Application remains stable.
No JavaScript errors occur.

TC_SORT01 Verify Featured Sorting
---------------------------------
Open the Product Category Listing page.
Click the Sort dropdown.
Select Featured.
Wait until products reload.
Verify the product order.

Expected Result

Products are displayed according to the Featured sorting logic.
Product order matches business requirements.
No duplicate products are displayed.

TC_SORT02 Verify Discount Sorting
----------------------------------
Open the Product Category Listing page.
Click the Sort dropdown.
Select Discount.
Verify the displayed product order.
Compare product discounts.

Expected Result

Products are sorted based on the highest discount.
Discount values appear correctly.
Sorting is applied successfully.

TC_SORT03 Verify Price Low to High Sorting
------------------------------------------
Open the Product Category Listing page.
Select Price: Low to High from the Sort dropdown.
Wait until products reload.
Verify the price of each displayed product.
Compare consecutive product prices.

Expected Result

Products are displayed in ascending price order.
No product is out of sequence.
Sorting is accurate across all displayed products.

TC_SORT04 Verify Price High to Low Sorting
------------------------------------------
Open the Product Category Listing page.
Select Price: High to Low from the Sort dropdown.
Wait until products reload.
Verify the displayed product prices.
Compare consecutive product prices.

Expected Result

Products are displayed in descending price order.
No incorrect ordering is observed.
Sorting is applied correctly.

TC_SORT05 Verify Sorting After Applying Filters
-----------------------------------------------
Open the Product Category Listing page.
Apply a price filter.
Click the Sort dropdown.
Select Price: Low to High.
Verify the filtered products.
Verify the sorting order.

Expected Result

Sorting is applied only to the filtered products.
Product order is correct.
Applied filters remain active.

TC_SORT06 Verify Sorting After Page Refresh
-------------------------------------------
Open the Product Category Listing page.
Select any sorting option.
Refresh the browser.
Observe the selected sorting option.
Verify product order.

Expected Result

Sorting behavior follows the business requirement.
Product order remains consistent.
No unexpected sorting behavior occurs.

TC_SORT07 Verify Sorting with Duplicate Prices
----------------------------------------------
Open the Product Category Listing page.
Select Price: Low to High.
Locate products having identical prices.
Verify their display order.
Refresh the page and verify consistency.
Expected Result
Products with identical prices are displayed consistently.
No product is missing or duplicated.
Sorting remains stable.

TC_SORT08 Verify Rapid Switching Between Sorting Options
--------------------------------------------------------
Open the Product Category Listing page.
Quickly switch between all sorting options multiple times.
Observe the loading behavior.
Verify the final selected sorting option.
Verify displayed products.

Expected Result

Application remains responsive.
Final selected sorting option is applied correctly.
No duplicate products or UI glitches occur.

TC_SORT09 Verify Empty Sort API Response Handling
-------------------------------------------------
Configure the sorting API to return an empty response.
Open the Product Category Listing page.
Select any sorting option.
Wait for the response.
Observe the product grid.

Expected Result

A "No Products Found" message is displayed.
Product grid remains empty.
Application remains stable.

TC_SORT10 Verify Invalid Sort API Response Handling
---------------------------------------------------
Configure the sorting API to return an invalid response.
Open the Product Category Listing page.
Select any sorting option.
Observe the application behavior.
Verify error handling.

Expected Result

The application handles the invalid response gracefully.
A meaningful error message is displayed.
No application crash or broken UI occurs.

TC_UI01 Verify Product Image Visibility
---------------------------------------
Open the Product Category Listing page.
Observe all displayed product cards.
Verify every product card contains an image.
Verify each image is fully loaded.
Verify images are displayed without distortion or cropping.

Expected Result

Every product card displays an image.
Images load successfully.
Images are clear and properly aligned.
No missing or broken images are displayed.

TC_UI02 Verify Broken Image Handling
------------------------------------
Open the Product Category Listing page.
Simulate or identify a product with an invalid image URL.
Refresh the page.
Observe the affected product card.
Verify the application's handling of the missing image.

Expected Result

A placeholder image is displayed instead of a broken image.
The page layout remains intact.
No broken image icon is displayed.
No JavaScript errors occur.

TC_UI03 Verify Product Name and Price Display
---------------------------------------------
Open the Product Category Listing page.
Verify each product card displays the product name.
Verify the product price is visible.
Compare the displayed details with the product data.
Scroll through the product listing.

Expected Result

Product names are displayed correctly.
Product prices are displayed correctly.
No product card has missing information.
Product details match the backend data.

TC_UI04 Verify Currency Format
------------------------------
Open the Product Category Listing page.
Observe the price displayed on each product card.
Verify the correct currency symbol is displayed.
Verify decimal formatting.
Compare with the application's currency standard.

Expected Result

Currency symbol is displayed correctly.
Price formatting is consistent.
Decimal values follow business requirements.
No formatting inconsistencies are observed.

TC_UI05 Verify Product Card Alignment
-------------------------------------
Open the Product Category Listing page.
Observe the alignment of all product cards.
Compare the spacing between adjacent cards.
Scroll through multiple rows.
Verify the overall layout consistency.

Expected Result

Product cards are properly aligned.
Equal spacing exists between cards.
No overlapping or misplaced cards are observed.

TC_UI06 Verify Product Grid Alignment
-------------------------------------
Open the Product Category Listing page.
Observe the product grid layout.
Verify equal spacing between rows and columns.
Scroll to the bottom of the page.
Verify grid consistency throughout the page.

Expected Result

Product grid remains consistent.
Rows and columns are properly aligned.
No broken layout is observed.

TC_UI07 Verify Responsive Grid Layout
-------------------------------------
Open the Product Category Listing page.
Resize the browser window gradually.
Observe the product grid.
Verify the number of product cards adjusts according to screen size.
Verify there is no UI overlap.

Expected Result

Product grid adjusts automatically.
Layout remains responsive.
No content overlap or horizontal scrolling occurs.

TC_UI08 Verify Hover Effect on Product Cards
--------------------------------------------
Open the Product Category Listing page.
Move the mouse pointer over a product card.
Observe the hover effect.
Repeat for multiple product cards.
Verify consistency across all products.

Expected Result

Hover effect is displayed correctly.
Animation is smooth.
Product card remains clickable.
Hover effect is consistent across all cards.

TC_UI09 Verify Duplicate Product Display
----------------------------------------
Open the Product Category Listing page.
Scroll through the complete product list.
Compare Product IDs or Names.
Identify any duplicate products.
Verify the uniqueness of displayed products.

Expected Result

No duplicate products are displayed.
Each product appears only once.
Product listing remains accurate.

TC_UI10 Verify Missing Product Information Handling
---------------------------------------------------
Open the Product Category Listing page.
Simulate a product with missing information.
Refresh the page.
Observe the affected product card.
Verify how the application handles incomplete data.

Expected Result

Missing information is handled gracefully.
Layout remains intact.
Placeholder text or default values are displayed where applicable.
No UI breakage occurs.

TC_RESP01 Verify Product Listing on Desktop
-------------------------------------------
Open the Product Category Listing page on a desktop browser.
Set the browser resolution to 1920 × 1080.
Verify the Filter panel is visible.
Verify the Sort option is displayed.
Verify the product grid is displayed correctly.

Expected Result

Product Listing page renders correctly.
Filter panel and Sort option are visible.
Product grid is properly aligned.
No UI overflow or broken layout is observed.

TC_RESP02 Verify Product Listing on Tablet
------------------------------------------
Open the Product Category Listing page on a tablet.
Verify the Filter panel behavior.
Verify the Sort option.
Verify the product grid layout.
Scroll through the product listing.

Expected Result

Product grid adapts to tablet resolution.
Filters and Sort options remain accessible.
UI elements are properly aligned.
No overlapping content is observed.

TC_RESP03 Verify Product Listing on Android Device
--------------------------------------------------
Open the Product Category Listing page on an Android device.
Verify the Filter option.
Verify the Sort option.
Scroll through the product list.
Rotate the device between Portrait and Landscape modes.

Expected Result

Product Listing page displays correctly.
Filters and Sort options function properly.
Layout adapts to orientation changes.
No UI distortion occurs.

TC_RESP04 Verify Product Listing on iPhone
------------------------------------------
Open the Product Category Listing page on an iPhone.
Verify the Filter option.
Verify the Sort option.
Scroll through the products.
Rotate the device between Portrait and Landscape modes.

Expected Result

Product Listing page displays correctly.
Product cards are responsive.
Filters and Sort options remain usable.
No layout issues or content clipping are observed.

TC_COMP01 Verify Product Listing Page on Google Chrome
-------------------------------------------------------
Open the Product Category Listing page in the latest version of Google Chrome.
Verify the page loads successfully.
Apply a price filter.
Apply a sorting option.
Verify the product cards are displayed correctly.

Expected Result

The page loads successfully.
Filters and sorting function correctly.
Product cards display without UI issues.
No browser-specific rendering problems are observed.

TC_COMP02 Verify Product Listing Page on Mozilla Firefox
---------------------------------------------------------
Open the Product Category Listing page in Mozilla Firefox.
Verify the page layout.
Apply a filter and sorting option.
Verify product cards.
Check for console errors.

Expected Result

The page functions correctly in Firefox.
UI elements render consistently.
No functional or layout issues occur.
No browser console errors are present.

TC_COMP03 Verify Product Listing Page on Microsoft Edge
------------------------------------------------------
Open the Product Category Listing page in Microsoft Edge.
Verify filters and sorting options are available.
Apply multiple filters.
Verify product listing updates.
Navigate between pages if pagination exists.

Expected Result

All page functionality works correctly in Edge.
UI rendering is consistent.
Product listing updates correctly after filtering.

TC_COMP04 Verify Product Listing Page on Safari
-----------------------------------------------
Open the Product Category Listing page in Safari.
Verify page loading.
Apply filters.
Change sorting options.
Verify product card rendering.

Expected Result

The page renders correctly in Safari.
Filters and sorting work as expected.
Product cards display correctly without layout issues.

TC_USAB01 Verify Filter Panel Usability
---------------------------------------
Open the Product Category Listing page.
Locate the Filter Panel.
Verify filter categories are clearly labeled.
Apply a filter without referring to documentation.
Observe the ease of interaction.

Expected Result

Filter panel is easy to locate.
Filter labels are meaningful.
Users can apply filters without confusion.
Overall interaction is intuitive.

TC_USAB02 Verify Sorting Option Usability
-----------------------------------------
Open the Product Category Listing page.
Locate the Sort dropdown.
Expand the sorting options.
Select different sorting values.
Observe the ease of changing sorting.

Expected Result

Sorting options are easy to locate.
Labels clearly describe the sorting method.
Sorting changes are simple and intuitive.

TC_USAB03 Verify Keyboard Navigation
------------------------------------
Open the Product Category Listing page.
Use the Tab key to navigate through interactive elements.
Focus on the Filter panel.
Select a filter using the keyboard.
Navigate to the Sort dropdown using the keyboard.

Expected Result

All interactive elements are accessible using the keyboard.
Focus indicators are visible.
Filters and sorting can be operated without using a mouse.

TC_PERF01 Verify Product Listing Page Load Time
-----------------------------------------------
Open the browser Developer Tools.
Clear browser cache.
Open the Product Category Listing page.
Measure the page load time.
Repeat the test three times.

Expected Result

The page loads within the acceptable performance threshold.
No unusually slow loading is observed.
Static resources load successfully.

TC_PERF02 Verify Filter Response Time
--------------------------------------
Open the Product Category Listing page.
Apply a price filter.
Measure the time taken for products to refresh.
Repeat with different price filters.
Compare response times.

Expected Result

Filter response time remains within acceptable limits.
Product updates occur smoothly.
No noticeable lag is experienced.

TC_PERF03 Verify Sorting Response Time
---------------------------------------
Open the Product Category Listing page.
Select Price: Low to High.
Measure the response time.
Select Price: High to Low.
Compare sorting response times.

Expected Result

Sorting completes within the expected response time.
Products reload smoothly.
No delays or UI freezing occur.

TC_PERF04 Verify Product Listing Under Slow Network
---------------------------------------------------
Enable Slow 3G network throttling.
Open the Product Category Listing page.
Apply a filter.
Change the sorting option.
Observe page responsiveness.

Expected Result

Loading indicators are displayed.
Application remains responsive.
Products load successfully after the network response.
No timeout or application crash occurs.

TC_LOAD01 Verify Product Listing with 100 Concurrent Users
-----------------------------------------------------------
Configure the load testing tool for 100 concurrent users.
Simulate users opening the Product Category Listing page.
Apply filters simultaneously.
Monitor server response time.
Record application performance metrics.

Expected Result

The application supports 100 concurrent users.
Response time remains within the acceptable limit.
No server failures or application crashes occur.

TC_LOAD02 Verify Product Listing with 500 Concurrent Users
----------------------------------------------------------
Configure the load testing tool for 500 concurrent users.
Simulate simultaneous page access.
Apply filters and sorting operations.
Monitor server resources.
Analyze performance metrics.

Expected Result

The application remains stable under load.
Server response time is acceptable.
No significant degradation in functionality occurs.

TC_LOAD03 Verify Simultaneous Filter Requests Under Load
--------------------------------------------------------
Configure multiple virtual users.
Simultaneously apply different price filters.
Monitor API response times.
Verify product listing updates.
Review server logs.

Expected Result

All filter requests are processed successfully.
No request failures occur.
Product data remains accurate.
Server performance remains stable.

TC_LOAD04 Verify Simultaneous Sorting Requests Under Load
---------------------------------------------------------
Configure multiple virtual users.
Simultaneously change sorting options.
Monitor API response time.
Verify sorted product listings.
Observe application stability.

Expected Result

Sorting requests are processed successfully.
Product order is correct for each request.
No data inconsistency occurs.
The application remains stable during peak activity.

TC_E2E01 Verify Complete Product Browsing Journey
-------------------------------------------------
Open the Product Category Listing page.
Verify products are loaded successfully.
Apply a Price Filter.
Verify filtered products are displayed.
Change the Sort option to Price: Low to High.
Verify products are sorted correctly.
Remove the applied filter.
Verify all products are displayed again.

Expected Result

The complete user journey executes successfully.
Filters and sorting work together correctly.
Product listing updates accurately throughout the flow.
No application errors occur.

TC_E2E02 Verify Multiple Filters with Sorting
---------------------------------------------
Open the Product Category Listing page.
Apply multiple price filters.
Verify filtered products are displayed.
Select Featured from the Sort dropdown.
Verify sorting is applied to the filtered products.
Remove one filter.
Verify the product listing updates correctly.

Expected Result

Multiple filters work correctly with sorting.
Product list updates accurately after every action.
No incorrect products are displayed.

TC_E2E03 Verify Browser Refresh During Active Filter
----------------------------------------------------
Open the Product Category Listing page.
Apply a price filter.
Select Price: High to Low sorting.
Refresh the browser.
Verify the page state after refresh.
Verify product listing.

Expected Result

Application behaves according to business requirements after refresh.
Product listing remains consistent.
No UI or functional issues occur.

TC_E2E04 Verify Browser Back and Forward Navigation
---------------------------------------------------
Open the Product Category Listing page.
Apply a filter.
Open any product detail page.
Click the browser Back button.
Verify previously selected filters.
Click the browser Forward button.
Verify the product detail page loads correctly.

Expected Result

Browser navigation preserves the application state.
Filters remain consistent.
Navigation does not break the application.

TC_E2E05 Verify Complete User Flow with No Products Found
---------------------------------------------------------
Open the Product Category Listing page.
Apply a filter that returns no products.
Verify the empty state message.
Click Clear All.
Verify the complete product list is restored.
Apply another valid filter.
Verify matching products are displayed.

Expected Result

Empty state is displayed correctly.
Application recovers successfully after clearing filters.
Valid filters continue to function correctly.

TC_MONKEY01 Verify Application Stability During Random Filter Clicks
--------------------------------------------------------------------
Open the Product Category Listing page.
Randomly click different filter options.
Randomly select and deselect filters.
Repeat for several minutes.
Observe the application behavior.

Expected Result

Application remains stable.
No crashes or UI corruption occur.
Product listing updates correctly.

TC_MONKEY02 Verify Application Stability During Random Sorting
--------------------------------------------------------------
Open the Product Category Listing page.
Randomly switch between sorting options.
Repeat the process multiple times.
Observe the product listing.
Monitor browser responsiveness.

Expected Result

Sorting continues to work correctly.
No duplicate products appear.
Application remains responsive.

TC_MONKEY03 Verify Random User Navigation
-----------------------------------------
Open the Product Category Listing page.
Randomly open product detail pages.
Navigate back to the listing page.
Refresh the page randomly.
Continue random navigation for several minutes.

Expected Result

Navigation remains smooth.
Product listing loads correctly.
No unexpected application errors occur.

TC_MONKEY04 Verify Random Combination of Filters and Sorting
------------------------------------------------------------
Open the Product Category Listing page.
Apply random price filters.
Select random sorting options.
Remove filters randomly.
Repeat the process continuously.

Expected Result

Application processes every action successfully.
Product listing remains accurate.
No UI inconsistencies occur.

TC_MONKEY05 Verify Random Page Scrolling and Refresh
-----------------------------------------------------
Open the Product Category Listing page.
Scroll randomly through the page.
Refresh the browser at random intervals.
Continue interacting with filters and sorting.
Observe application stability.

Expected Result

Application remains stable throughout random interactions.
Product listing loads correctly after refresh.
No rendering issues are observed.

TC_GORILLA01 Verify Repeated Filter Apply and Remove
----------------------------------------------------
Open the Product Category Listing page.
Apply a price filter.
Remove the applied filter.
Repeat the process 50 times.
Observe application performance.

Expected Result

Filter functionality remains consistent.
No performance degradation occurs.
Application remains stable.

TC_GORILLA02 Verify Repeated Sorting Operations
-----------------------------------------------
Open the Product Category Listing page.
Change the sorting option repeatedly.
Cycle through every available sorting option.
Repeat the process 50 times.
Observe application behavior.

Expected Result

Sorting works correctly throughout the test.
No incorrect product ordering occurs.
Application remains responsive.

TC_GORILLA03 Verify Continuous Page Refresh
-------------------------------------------
Open the Product Category Listing page.
Refresh the browser repeatedly.
Continue refreshing for several minutes.
Observe page loading.
Verify filters and sorting after the final refresh.

Expected Result

Application loads successfully after every refresh.
No session or UI issues occur.
Product listing remains accurate.

TC_GORILLA04 Verify Long Duration Filter and Sorting Operations
---------------------------------------------------------------
Open the Product Category Listing page.
Continuously apply and remove filters.
Continuously change sorting options.
Repeat the process for an extended period (30–60 minutes).
Monitor browser memory usage and application responsiveness.

Expected Result

Application remains stable during prolonged use.
No memory leaks are observed.
UI remains consistent throughout the test.

TC_GORILLA05 Verify Recovery After Prolonged Usage
--------------------------------------------------
Use the Product Category Listing page continuously for an extended period.
Apply filters, sorting, scrolling, and navigation repeatedly.
Refresh the page after prolonged usage.
Verify all page components.
Verify product listing accuracy.

Expected Result

Application recovers successfully after prolonged usage.
All functionality continues to work correctly.
No crashes, memory leaks, or UI inconsistencies are observed.
