QA Manual Test Cases:-

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

AI Manual Test Cases ----------------------------------------------


																						
