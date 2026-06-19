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

