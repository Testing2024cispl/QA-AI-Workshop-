Member :- Sagarika Sahu


Website:-Grocery Store Demo - Online Store 

Human Thinking Test Cases

TestCases_001:-  Login Flow

1.Go to https://grocerystoredemo.pcubeweb.com

2.Verify Homepage loads successfully.

3.Click on Account icon.

4.Verify Sign In popup is displayed.

5.Verify Country Code (+91) is displayed by default.

6.Verify Phone Number input field is displayed.

7.Verify Send OTP button is displayed.

8.Enter a valid mobile number.

9.Click on Send OTP.

10.Verify OTP Verification popup is displayed.

11.Verify six OTP input fields are displayed.

12.Verify OTP input fields accept numeric values only.

13.Enter valid OTP. 

14.Verify login is successful. 

15.Verify Account section is accessible. 

TestCases_002:- End-to-End Login Flow with user should be able to get OTP through Whatsapp

1.Go to https://grocerystoredemo.pcubeweb.com

2.Verify Homepage loads successfully.

3.Click on Account icon.

4.Verify Sign In popup is displayed.

5.Verify Country Code (+91) is displayed by default.

6.Verify Phone Number input field is displayed.

7.Verify Send OTP button is displayed.

8.Enter a valid mobile number.

9.Click on Send OTP.

10.Verify OTP Verification popup is displayed.

11.Verify that the timer should get displayed

12.Verify "Didn't get the code? Send it on WhatsApp" option is displayed when user not get the OTP on phone number

13.Verify that the WhatsApp button is enabled and clickable

14.Verify OTP countdown timer is displayed.

15.Enter valid OTP.

16.Verify OTP is accepted successfully.

17.Verify OTP popup closes automatically.

18.Verify user is logged in successfully.

19.Verify Account section is accessible.

TestCases_003:- Verify Login Flow with Invalid Inputs

1.Open https://grocerystoredemo.pcubeweb.com

2.Click on Account icon.

3.Leave the mobile number field blank.

4.Click Send OTP.

5.Verify validation message is displayed.

6.Enter a mobile number with less than 10 digits.

7.Click Send OTP.

8.Verify validation message is displayed.

9.Verify that phone number text field should not accept alpha numeric , Special character

10.Enter a valid mobile number.

11.Click Send OTP.

12.Verify OTP Verification popup is displayed.

13.Enter an invalid OTP.

14.Verify error message is displayed.

15.Enter an incomplete OTP (less than 6 digits).

16.Verify OTP verification is not allowed.

17.Verify only numeric values are accepted.

18.Verify special characters are not accepted.

19.Wait for OTP to expire.

20.Enter expired OTP.

21.Verify OTP expired message is displayed.

22.Attempt multiple invalid OTP submissions.

23.Verify appropriate error/security message is displayed.

AI Manual Test Cases:-

Member :- Sagarika Sahu

Prompt:- Write End-to-End Login Flow Test Case for grocerystoredemo.pcubeweb.com

TestCases_001:-

Launch Grocery Store Website.

Click Account.

Enter Valid Mobile Number.

Request OTP.

Enter Valid OTP.

Complete Login.

Verify User Account Access.

Verify Session Persistence.

My thoughts:-

● What I felt Suitable:-

Covers complete login journey.

Includes OTP authentication.

Verifies successful user login.

● What I felt Not Suitable:-

Missing invalid OTP scenarios.

Missing WhatsApp OTP fallback flow. 

Missing OTP resend validation.

Missing phone number validation.

Missing OTP field validation.

Final Test Case:-

AI + Manual Combined (Automation Ready)

Open Grocery Store Demo Website.

Verify Homepage loads successfully.

Click Account icon.

Verify Login popup appears.

Verify +91 country code is displayed.

Enter valid mobile number.

Click Send OTP.

Verify OTP Verification popup appears.

Verify mobile number is displayed correctly
.
Verify six OTP input boxes are displayed.

Verify OTP timer is displayed.

Verify WhatsApp OTP option is displayed.

Enter valid OTP.

Verify login is successful.

Verify popup closes automatically.

Verify Account section is accessible.

Refresh the page.

Verify logged-in session persists.

Navigate to Account page.

Verify user information is displayed correctly.

Capture screenshots and logs for reporting.

Mark test as Passed if all validations succeed.

QA Manual Test Cases:-

Member :- Sagarika Sahu

Website:- https://grocerystoredemo.pcubeweb.com

Human Thinking Test Cases

TestCases_004:- Search Suggestion and Add To Cart Flow

Open https://grocerystoredemo.pcubeweb.com

Verify Homepage loads successfully.

Click inside the Search Bar.

Verify Search Suggestion popup is displayed.

Verify Bestseller Categories are displayed.

Verify Category Name and Category Image are visible.

Select "Biscuits & Snacks" category from suggestions.

Verify category products are displayed.

Select a product from the category.

Verify Product Name, Image and Price are displayed correctly.

Click ADD button.


Verify product is added successfully.

Verify Cart count increases.

Click Cart icon.

Verify selected product appears in cart.

Verify Product Name, Quantity and Price.

Verify that user is able to increase/ decrease  quantity 

Verify that user is able to remove the added to cart product

Verify Cart Total is calculated correctly.

TestCases_005:- Search Product and Add To Cart Flow

Open Grocery Store Demo Website.

Click Search Bar.

Enter product name "Lays".

Verify matching products appear.

Select the product from search results.

Verify product details.

Click ADD button.

Verify product is added to cart.

Open Cart page.

Verify added product details.

Verify quantity is 1.

Verify that user is able to increase/ decrease  quantity in the cart

Verify that user is able to remove the added to cart product

Verify total amount calculation.

TestCases_006:- Invalid Search Flow

Open Grocery Store Demo Website.

Enter an invalid product name in the search bar.

Click Search 

Verify no matching products are displayed.

Verify appropriate message is shown .

Clear the search field.

Verify product listing is restored

AI Manual Test Cases:-

Member :- Sagarika Sahu

Prompt:- Write test case for Search Suggestion and Add To Cart functionality

Open Website.

Click Search Bar.

Verify category suggestions.

Select category.

Open product.

Add product to cart.

Verify cart count.

Verify cart details.

Your thoughts:-

● What I felt Suitable:-

Covers Search Suggestion functionality.

Covers Category navigation.

Covers Add To Cart functionality.

Covers Cart validation.

● What I felt Not Suitable:-

Missing product search validation.

Missing cart calculation verification.

Missing category selection validation.

Final Test Case:-

AI + Manual Combined (Automation Ready)

Open Grocery Store Demo Website.

Verify Homepage loads successfully.

Click Search Bar.

Verify Bestseller Categories popup appears.

Verify category images and names are displayed.

Select a category from suggestions.

Verify category page/products load successfully.

Select a product.

Verify Product Name, Image and Price.

Click ADD button.

Verify Cart count increases.

Open Cart page.

Verify selected product is displayed.

Verify Quantity and Price.

Verify Cart Total calculation.

Capture screenshots and logs.

Mark test as Passed if all validations succeed.









