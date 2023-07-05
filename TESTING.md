# Testing
* [Back to README Home page](/README.md)
#
- [Manual Testing](#manual-testing)
    - [Responsive Testing](#responsive-testing)
    - [Lighthouse Testing](#lighthouse-testing)
    - [Browser Testing](#browser-testing)
    - [User Stories Testing](#user-stories-testing)
- [Code Validation](#code-validation)

## **Manual Testing**

* This site was tested manually by:
    - Testing the UI and functionality of features for different device sizes and browsers.
    - Evaluating performance and loading times using lighthouse and interacting wiht the site as a user.
    - Ensuring that user story features are functioning as they should be with the expected outcome from specific user actions.
    - All links and user pathways function as intended and navigate the user as expected through the site.
* The details of how the manual testing was carried out can be seen below.
* I have also included the code validation in the TESTING document.

## Responsive Testing
<details>
<summary>👇</summary>

* Site resonsivity was tested using google chrome DevTools and with my own Galaxy S20 FE.
* The screenshot below shows a list of the devices that were tested via chrome devtools:


    ![responsive](readme/desktop-testing/devtools-responsive-testing.png)

[Back to top](#testing)

* The site was shown to be fully responsive, readable and functional on all of the tested devices.
* The "trekkers" site name navlink in the navbar is set to be hidden in screen sizes under 365px in order to prevent the navbar UI becoming crowded and distorted.
*  In Chrome devtools most mobile screen sizes are still wide enough to display the "trekkers" heading.
* The screens where it is hidden are :
    - Samsung galaxy S8+
    - Galaxy fold
* On my own phone model (Galaxy S20 FE), the "trekkers" navlink heading is hidden.

* Site resposivity was also tested on Amiresponsive as seen in the README.
* Below is a screenshot of the viewport sizes tested on amiresponsive:

 ![amiresponsive](readme/desktop-testing/amiresponsive-viewport-sizes.JPG)

* I also included some screenshots of features in mobile size in the user story testing to show the responsive design. 

[Back to top](#testing)
</details>

- - -
## Lighthouse testing

<details>
<summary>👇</summary>

* Lighthouse testing in chrome DevTools showed an overall performance of 99% and good SEO and Accessibility scores.
* There were some suggestions to improve best practice scores which will be added to the future features for this site.

    ![Lighthouse results](static/readme/testing/lighthouse-testing.JPG)

[Back to top](#testing)
</details>

- - -

## Browser testing

<details>
<summary>👇</summary>

* The site was developped using Google Chrome browser and tested in Firefox and Microsoft Edge.


[Back to top](#testing)
</details>

- - -

## User Stories Testing

<details>
<summary>👇</summary>

The User Stories and features were continuously tested during development and this testing is documented here with screenshots of the features from the deployed site.


### Epic 1: Authentication


<details>
<summary>User Stories test cases</summary>
<br>

#### **User Stories**
1. Sign up: As a **user** I can **create an account** so that I can **access all the site features**
    - Sign up page allows new users to create an account.
    - Handles errors for duplicate username, blank fields or mismatching passwords.
    - Tested all links working as normal. 
    - The link to the sign in page will redirect user to sign in page.
    - If all form fields are valid and user clicks sign up they will be redirected to the sign in page.

    ![sign-up](/readme/desktop-testing/sign-up-page.JPG)
    ![sign-up-existing-user](/readme/desktop-testing/sign-up-form-existing-username-error.JPG)
    ![sign-up-errors](/readme/desktop-testing/sign-up-different-password.JPG)


[Back to top](#testing)

#
2. Sign in: As a **user** I can **login** so that I can **access features only available to logged in users **

    - Sign in page allows users who have created an account to sign in in order to access all the site features.
    - Handles errors for incorrect credentials and blank fields.
    - Tested all links working as normal. 
    - The link to the sign up page will redirect user to sign up page as expected.
    - If all form fields are valid and user clicks sign in, they will be redirected to the homepage.

    ![sign-in](readme/desktop-testing/sign-in-page.JPG)
    ![sign-in-empty-fields](readme/desktop-testing/sign-in-empty-fields.JPG)
    ![sign-in-missing-user](readme/desktop-testing/sign-in-page-missing-username.JPG)
    ![sign-in-blank-password](readme/desktop-testing/sign-in-blank-password.JPG)
    ![sign-in-wrong-credentials](readme/desktop-testing/sign-in-wrong-password.JPG)


[Back to top](#testing)
#

3. Sign out: As a **user** I can **logout** so that I can **exit my account and prevent others from gaining access**
    - The Navbar displays a sign out button to logged in users so that they can sign out from any page in the site.

    ![desktop-logged-out-nav](readme/desktop-testing/logged-in-nav.JPG)

    - When the user clicks the sign out button they are redirected to the home page.
    - Once logged out the Navbar will change to reflect the users ogged out status and provides the links to sign in and sign up.

    ![desktop-logged-out-nav](readme/desktop-testing/logged-out-nav.jpg)


[Back to top](#testing)
#
4. Refreshing access tokens: As a **user** I can **maintain my logged in status for 24 hours** so that I can **easily interact with the app throughout the day**.

    - Unless users click the sign out button, they remain logged in for 24 hours.

[Back to top](#testing)

#

5. Create admin panel: As a **site owner** I can **access the admin panel** so that **I have access to all site features and functionality**.anel can be accessed by those with the superuser credentials.

  - This is a Backend api feature, please see the relevant readme [here](https://github.com/HPCarey/pp5-trekkers-api).

[Back to top](#testing)

6. Create superuser: As a **site owner** I can **create a superuser** so that **I can give admin users access to the admin panel**.

  - This is a Backend api feature, please see the relevant readme [here](https://github.com/HPCarey/pp5-trekkers-api).

[Back to top](#testing)

</details>

- - -

### Epic 2: Navigation


<details>
<summary>User Stories test cases</summary>
<br>

#### **User Stories**
7. As a **user** I can **quickly view my logged in/out status in the navbar** so that I can **decide on my next action**

    - The Navbar displays a home, sign in and sign up link to logged out users so they can choose to interact with the site on a read only basis or sign in/up to access more features
    ![desktop-logged-out-nav](readme/desktop-testing/logged-out-nav.jpg)

    - Once signed in the navbar gives the user access to other actions and pages such as add post, liked posts, feed and the users profile link with their avatar.
    ![desktop-logged-out-nav](readme/desktop-testing/logged-in-nav.JPG)

[Back to top](#testing)
#
8. Routing: As a **user** I can **view the navbar on every page** so that I can **easily navigate through the site**.

    - The Navbar has been tested on every page and in different screen sizes. 
    - The navbar is fully responsive and fully functional.
    - Active navlinks are in green  to help the user know which page they are currently on.
    - When the user hovers over a navlink it will go green like the active navlink to help user know which link their mouse is over.
    - Both the logo and site name act as home navlinks to make it convenient and easy to get back to the home page.

    ![mobile-nav](readme/desktop-testing/mobile-nav-sm.jpg) 
    ![mobile-logged-out](readme/desktop-testing/mobile-nav-logged-out.jpeg) 
    ![mobile-logged-in](readme/desktop-testing/mobile-logged-in-nav-sm.jpg)

[Back to top](#testing)
#

9. Conditional Rendering: As a **logged out user** I can **view sign in and sign up options** so that I can **easily tell whether I am logged in and can log in easily if not**.

    - Already established in test case 7.

[Back to top](#testing)

10. Avatar: As a **logged in user** I can **view my profile link and avatar image on the navbar** so that I can **quickly see that I am logged in”

    - Already established in test case 7.

[Back to top](#testing)

11. Popular profiles list: As a **logged in user** I can **view other user’s profile names and avatars** so that I can **easily identify and follow other users**

    - The popular profiles list is displayed on the right of the screen for desktop users and at the top just under navbar for mobile users.
    - Profile avatars act as links to other users profiles, all these links have been tested and redirect to the correct profiles.

    ![popular-profiles](readme/desktop-testing/popular-profiles.jpg)![mobile-popular-profiles](readme/desktop-testing/mobile-popular-profiles.jpg)

[Back to top](#testing)

</details>

- - -

### Epic 3: Posts


<details>
<summary>User Stories test cases</summary>
<br>

#### **User Stories**
12. Create a post: As a **logged in user** I can **create a new post** so that I can **share my experiences and suggestions for good hikes and walks I’ve been on**.

    - Logged in users have access to the add post form and can create a post about their trail.

         ![add-post-form](readme/desktop-testing/add-post-page.JPG)
    
    - Each add post form handles errors for blank, required fields and for incorrect field values.

        ![add-post-form-errors](readme/desktop-testing/add-post-error-message.JPG) 
        ![add-post-form-errors](readme/desktop-testing/form-field-error.JPG) 
        ![add-post-form-rating-error](readme/desktop-testing/rating-value-error.JPG) 


    - Images over 2mb will throw an error to conserve cloud storage space.
            ![add-post-form-errors](readme/desktop-testing/image-too-large-error.JPG)

    - Once an image has been uploaded to the form a change image utton will appear to allow user to change the image.
        ![add-post-form](readme/desktop-testing/change-image-button-diff-dropdown.JPG)
    - There is a dropdown menu containing 4 choices of difficulty level with the default value set to easy.

        ![difficulty-dropdown](readme/desktop-testing/difficulty-dropdown.jpg)

    - A star rating value is also requires a value of at least 1 out of 5 stars.

        ![add-post-form-end](readme/desktop-testing/end-of-add-post-form.JPG)

    - Once the user clicks create and all fields are valid, the post will be published to the homepage and the user's profile page.
    - Once the user clicks create they are redirected to the post detail page, where they can take further actions related to the post.
    - If the user clicks cancel instead of create, they will be redirected to the home page instead.


[Back to top](#testing)

13. Edit a post: As a **logged in user** I can **edit my post** so that I can **revise my content**

    - Post owners have the ability to edit their posts from the post detail page via the three dot dropdown menu.

        ![edit-post-form](readme/desktop-testing/post-detail-three-dots-sm.jpg)

    - The edit form has all the original values pre-populated in the form fields, with the exception of the star rating value which does not display the stars filled in. 
        - note: the original value is still passed to the edit form and if the user adjusts other values the original rating value will remain, but it is an unsolved bug that the stars don't display the value in the edit form. 
    - The same field errors are handled as in the add post form but as the fields are pre-populated the blank field error only occurs for trail name and country when the user physically deletes the value and leaves them blank. 
    - All fields have been tested to see if the edited value is updated as expected and in each case they pass. 
    - If all form fields are valid and the user clicks save, they are redirected to the post detail again.
    - If the user clicks cancel in this case they will be redirected to the post details page.

    ![edit-post-form](readme/desktop-testing/edit-form.JPG)


[Back to top](#testing)

14. Delete a post: As a **logged in user** I can **delete my post** so that I can **remove content I have posted**

    - Post owners have the ability to delete their posts via the post detail page.
    - Post detail displays a three dot dropdown menu to users who are the post owner.
    - If the user clicks delete the post will be removed from the site and the user will be redirected to whatever page they navigated to the posts detail from, ie. their own profile or the home page.
    - In the Backend API the post model has an ondelete cascade so all comments and likes associated with the post will be deleted.

    ![delete-post-form](readme/desktop-testing/post-detail-three-dots-sm.jpg)


[Back to top](#testing)

15. View all posts: As a **user** I can **view all posts** so that I can **see what trails other users have walked and how they were**

    - All posts are avaialable to be viewed by both logged-in and logged-out users via the home page.

    ![loggged-out-home](readme/desktop-testing/logged-out-home.JPG)


[Back to top](#testing)

16. View post detail: As a **user** I can **view individual post details** so that I can **view other details and comments about the post**

    - All users can view the post detail of individual posts.
    - All users can view the comments under the post and see how many likes the post has. 
    - Only logged in users will have the ability to post a comment or like a post.

        ![loggged-out-post-detail](readme/desktop-testing/logged-out-post-detail.JPG)


[Back to top](#testing)

17. Like a post: As a **logged in user** I can **like a post** so that I can **quickly show my appreciation for another users content**

    - Logged-in users can like posts via the home page, post detail page or their feed.

            
        ![liked-no-results](readme/desktop-testing/liked-no-results.JPG)
        ![liked-after-liking](readme/desktop-testing/liked-after-liking.JPG)

    - Clicking the heart icon will add the post to liked posts and fills in the heart icon with a red color.
    - The likes count for the post will go up by 1.
    - Clicking the heart icon again will remove the post from liked posts and will remove the filled in red colour.
    - The likes count for the post will go down by 1.

        ![unliked-post](readme/desktop-testing/unliked-post.jpeg)

        ![liked-post](readme/desktop-testing/liked-post.jpeg)
    

    - Logged-out users cannot like posts.
    ![log-in-to-like](readme/desktop-testing/log-in-to-like.png)

    - Users cannot like their own posts.

         ![cant-like-own](readme/desktop-testing/cant-like-your-own.png)

[Back to top](#testing)


18. View liked posts: As a **logged in user** I can **view liked posts** so that I can **easily find the posts about trails that interested me**

    - Logged-in users can view their liked posts page to easily find trails they are interested in and want to keep easily accessible by liking.
            
        ![liked-after-liking](readme/desktop-testing/liked-after-liking.JPG)
        ![mobile-liked](readme/desktop-testing/mobile-liked-sm.jpg)


[Back to top](#testing)

19. Search posts: As a **user** I can **search posts** so that I can **find a post by author, trail name or location**

    - The search bar allows users to search for posts by keywords including post author, location, country, trail name, difficulty.
    - It funtcions and displays correclty on all screen sizes, on the homepage, feed and liked page. 
   
      ![search-bar](readme/desktop-testing/search-bar.jpg)
      ![search-bar-mobile](readme/desktop-testing/mobile-popular-profiles.jpg)

     - The search function returns relevant posts as expected according to the user's search words.
        ![search-location](readme/desktop-testing/search-location.JPG)
        ![search-difficulty](readme/desktop-testing/search-difficulty.JPG)


     - User's can also refine the search by using more than one keyword.

        ![search-multiple](readme/desktop-testing/search-multiple-key-words.JPG)

    - If the users search keywords don't match any posts an error message is displayed iinforming the user to adjust the search term. 
            
        ![no-search-results](readme/desktop-testing/search-no-results.JPG)
        


[Back to top](#testing)

</details>

- - -

### Epic 4: Comments

<details>
<summary>User Stories test cases</summary>
<br>

#### **User Stories**
20. Create a comment: As a **user** I can **leave a comment under a post** so that I can **express my opinion and engage with the content and the community**

    - Logged-in users have access to a comment form via the post detail page.
    - Clicking the comment icon underneath a post will redirect the user straight down to the comments form on the post detail page, but the user can also access it by simply clicking on the post and scrolling down manually.

        ![comment-form](readme/desktop-testing/comment-form.JPG)

    - Once a user types something and clicks post in the comment form, the post detail page will display the newly published comment. 

        ![comment-test](readme/desktop-testing/comment-test.JPG)
        ![comment-test-result](readme/desktop-testing/comment-test-result.JPG)

[Back to top](#testing)

21. Comment date: As a **user** I can **see the comment date** so that I can **know how long a go a comment was left**

    - The amount of time since the comment was first created or last updated is published beside the comment to show users how old the comment is.

        ![old-comment](readme/desktop-testing/old-comment.JPG)
        ![updated-comment](readme/desktop-testing/updated-comment.JPG)

[Back to top](#testing)

22. View comments: As a **user** I can **view other comments** so that I can **see what others have said**

    - As mentioned in previous test cases, both logged-in and logged-out users can view comments made by other users under the post. 

        ![logged-out-post-detail](readme/desktop-testing/logged-out-post-detail.JPG)
        ![comment-test-result](readme/desktop-testing/comment-test-result.JPG)

[Back to top](#testing)

23. Edit comments: As a **user** I can **edit my comment** so that I can **revise the information**

    - If the user is the owner of a comment, a three dot dropdown will be displayed in the right hand corner of the published comment.
    - This dropdown menu contains the icon-link to open the edit comment form. 
    ![comment-edit icon](readme/desktop-testing/comment-view.JPG)
    ![edit-comment-form](readme/desktop-testing/edit-comment-form.JPG)
    - If the user makes a change to the comment and clicks the save button, the post detail page will display the updated comment and updated time. 
    - If the user clicks cancel, the post detail page will display the original comment.

        ![old-comment](readme/desktop-testing/old-comment.JPG)
        ![updated-comment](readme/desktop-testing/updated-comment.JPG)

[Back to top](#testing)

24. Delete comments: As a **user** I can **delete my comment** so that I can **remove it from the post**

    - The delete icon is also available to comment owners via the three dot dropdown.
    - If the user clicks the delete icon, the comment is removed from the post detail page and the comments count goes down by 1. 
    ![delete-comment](readme/desktop-testing/delet-comment.JPG)
    ![deleted-comment](readme/desktop-testing/deleted-comment.JPG)

[Back to top](#testing)


</details>

- - -

### Epic 5: Profiles

<details>
<summary>User Stories test cases</summary>
<br>

#### **User Stories**
25. Profile page: As a **user** I can **view another user’s profile page** so that I can **see their posts and their bio**

    - Both logged-in and logged-out users have access to other users' profile pages.
    - Logged-in users will have access to a follow/unfollow button and edit dropdown menu for their own profile. 
        ![profile-logged-out](readme/desktop-testing/profile-logged-out.JPG)
        ![profile-logged-in](readme/desktop-testing/profile-logged-in.JPG)

[Back to top](#testing)

26. User stats: As a **user** I can **see stats via a user profile** so that I can **see how many posts/followers/following they have**

    - The stats on the users profile show how many posts and followers the profile owner has, as well as how many profiles they are following.
    - The followers count goes up by one if the current user clicks follow.
    - The followers count goes down by one if the current user clicks unfollow. 

        ![follow-count](readme/desktop-testing/follow-count.JPG)
        ![unfollow-count](readme/desktop-testing/unfollow-count.JPG)

    - The same applies to the following count if the profile owner follows/unfollows another user, the following count goes up or down in response.

        ![following-count](readme/desktop-testing/folloing-count.JPG)
        ![unfollowing-count](readme/desktop-testing/unfollowing-count.JPG)

    - Similarly, the posts count goes up when a user adds a post and goes down when apost is deleted.
    - If the user has not posted anything, there is a message explaining that the profile owner has no posts.
        
        ![profile-no-posts](readme/desktop-testing/profile-no-posts.JPG)
            
        ![unfollowing-count](readme/desktop-testing/profile-page-with-post.JPG)


[Back to top](#testing)

27. Follow/Unfollow a user: As a **logged in user** I can **follow other users whose content is more relevant or meaningful to me** so that I can **view content filtered by the users I follow**

    - As seen above, logged-in users have access to a follow button so that they can follow users whose content they enjoy.
    -The follow button toggles between follow and unfollow depending on whether the user currently follows the given profile or not. 
    - The posts of profile owners that the current user follows will be added to their feed, so they can easily see when a user they follow posts new content.
    - If the current logged-in user doesn't follow any profiles, their feed will display a message suggesting that they follow a profile. 

        ![feed-no-results](readme/desktop-testing/feed-no-results.JPG)
        
        ![feed-after-following](readme/desktop-testing/feed-after-following.JPG)

[Back to top](#testing)

28. Edit Profile: As a **user** I can **edit my profile** so that I can **update my personal details**

    - If the current logged-in user is the owner of a profile, a three dot dropdown will be displayed in the Profile header
    - This dropdown menu contains the icon-links to edit the profile, change the username and change the password. 

        ![edit-profile-dropdown](readme/desktop-testing/edit-profile-dropdown.JPG)
   
    - The edit profile link will take the user to an edit profile form.

    - The user can add an avatar image and bio via this form.

    ![edit-profile](readme/desktop-testing/edit-profile-form.JPG)

    - Both the image and bio field are optional, if left blank and the user clicks save they will simply be redirected to the their profile page.
    - If they enter values for these fields and click save they will be redirected to their profile page which will now display the new image/bio values. 
    - If the user enters values for these fields and clicks cancel, they will be redirected to the profile page with no changes reflected in the profile.

        ![Filled-profile](readme/desktop-testing/profile-edit-form-filled.JPG)

        ![updated-profile](readme/desktop-testing/profile-no-posts.JPG)

[Back to top](#testing)

29. Update username and password: As a **user** I can **update my username/password** so that I can **make alterations as needed**

    - The three dots dropdown menu "change username" link redirects user to a simple form where they can update their username. 

        ![edit-username](readme/desktop-testing/change-username-form.JPG)

    - If the user clicks save without making any changes, the form throws an error message.

        ![already-username-error](readme/desktop-testing/username-blank.JPG)

    - If the user attempts to use an invalid symbol, a space or more than 150 characters, the form will throw an error message. 

        ![username-error](readme/desktop-testing/change-username-error-too-many-chars.JPG)
        ![username-more-error](readme/desktop-testing/username-error-message.JPG)

    - If the user clicks cancel, whether or not they have made changes to the username, they will be redirected to their profile with no changes to the username.
    - If the user makes a valid change to the username and clicks save, they will be rediredted to their profile page where their username will have been updated.
    - The Profile navlink and popular profiles link will also reflect this change to the username.
    - The user will now be required to sign in with this new username.
    
     ![edited-username](readme/desktop-testing/edited-username.JPG)

    - The three dot dropdown "change password" link redirects user to a simple form where they can update their password. 

     ![password-form](readme/desktop-testing/change-password-form.JPG)

     - If the user inputs passwords that don't match, the form will throw an error.

     ![password-form-error](readme/desktop-testing/edit-password-error.JPG)

     - If the user clicks save and the fields are blank the form will throw the following error: 

     ![password-form-blank](readme/desktop-testing/edit-password-blank-fields.JPG)

     - If the user tries to put a password that is longer than 128 characters, then the form will throw the following error:

     ![password-form-blank](readme/desktop-testing/password-too-many-char-error.JPG)

     - Once the user inputs two valid, matching passwords, they will be redirected to the profile page.
     - If the new password is the same as the current password, no error will occur, the user will be redirected to their profile page and can continue to use the same password. 
     - The user will now need to sign in using the new, updated password. 


[Back to top](#testing)


</details>
</details>

- - -

## Code Validation

<details>
<summary>👇</summary>

1. ### **HTML Validation**

HTML validation was done using 
[W3C Markup Validator](https://validator.w3.org/). In order to validate the HTML without getting errors due to the Django template tags, the following steps were followed:

1. Navigate to the deployed site url using the google chrome browser.
2. Navigate to the page of the site you want to validate.
3. Right click anywhere on said page and select "View page source".
4. Copy the source code and open the validator.
5. Select Validate by direct input and paste the code into the validator field and click "Check"

Below are the issues encountered during initial validation: 

**Home Page**

* A warning to add a language attribute to the html tag
* Several Info messages to remove trailing / from self-closing elements like img and link. 
* I discovered that these / were getting added automatically whenever I used the prettier command to tidy up the template code. 
    ![home-page](static/readme/testing/code-validation/hmtl-val-homepage.JPG)

    ![all-messages](static/readme/testing/code-validation/trailing-slash-errors.JPG)

* The results after cleaning up these issues and re-deploying to heroku contain no errors:

    ![all-messages](static/readme/testing/code-validation/html-homepage-final.JPG)


[Back to top](#testing)

**Sign in Page**

* No errors

**Sign up Page**

* No errors

**Sign out Page**

* No errors

**Add booking form page**

* An attribute error for using "placeholder" with date input. The source of this error was in the forms.py date widget. I simply removed the placeholder attribute.
* The end tag error and unlcosed element were related. Both errors were dealt with upon locating the unclosed div and closing it.

    ![booking-page](static/readme/testing/code-validation/booking_form_validator_errors.JPG)

* The final results after addressing these issues contain no errors:

    ![booking-page](static/readme/testing/code-validation/add_booking-final.JPG)

[Back to top](#testing)

**Update booking form page**

* Unsurprisingly the same unclosed div error results occured on this page as the one in the booking form page. Since I create the update form template by copy, pasting and making adjustments to the booking form, this was expected and fixed in the same manner.


    ![booking-page](static/readme/testing/code-validation/update_booking_error.JPG)

* Final results after fixes:

    ![booking-page](static/readme/testing/code-validation/update_booking-final.JPG)


[Back to top](#testing)

**User Profile page**

* No errors


**Cancel appoinment confirmation page**

* An empty attribute value error for the form attribute action="".

    ![booking-page](static/readme/testing/code-validation/cancel_confirmation_error.JPG)

* Results after removing the unneeded attribute:

    ![booking-page](static/readme/testing/code-validation/cancel-page-final.JPG)


**404 page**

* No errors

[Back to top](#testing)
#

2. ### CSS Validation
CSS Validation was done using [Jigsaw](https://jigsaw.w3.org/css-validator/)

* One error occured for the .btn-secodary class. Too many values. 
* I am not 100% sure, but I think perhaps this error occured becasue I had already targeted the buttons with these rules somewhere else already.

![CSS](static/readme/testing/code-validation/css-validator-error.JPG)

* After playing around with this css for a bit I realised that the particular rule was not really making a differnece to the display and after commenting it out to be sure I decide to delete it.
* After double checking all my styles were working ok, I ran the css through the validator again and it came up clean.

![CSS_no_error](static/readme/testing/code-validation/css-validator-fixed.JPG)

[Back to top](#testing)

#

3. ### Python Validation
 Python Validation was done using the [CI Python Linter](https://pep8ci.herokuapp.com/).
 I used the gitpod problems tab to minimise python code errors as I went along, so there were not that many errors to address from passing the code through the linter. 

#### **Profject files**

**settings.py**
* Initial warnings for this file were as seen in this screenshot:

    ![settings-warning](static/readme/testing/python-code-validation/settings_warnings.JPG)

* The settings.py line too long warnings are from the django password validators. 
    ![settings-warning](static/readme/testing/python-code-validation/auth-password-validators.JPG)

* After consulting my own mentor and other mentors on slack, I left the too long lines in this particular case as they are part of the django automated code and splitting the string up might lead to unforseen issues. 
* The final validation results look like this:

    ![settings-warning](static/readme/testing/python-code-validation/settins_final.JPG)

[Back to top](#testing)

**urls.py**
* No errors found

    ![settings-warning](static/readme/testing/python-code-validation/urls-main.JPG)

[Back to top](#testing)
#### **Booking app files**

**admin.py**
* No errors found

    ![settings-warning](static/readme/testing/python-code-validation/adming-no-errors.JPG)

[Back to top](#testing)

**forms.py**
* No errors found

    ![settings-warning](static/readme/testing/python-code-validation/forms_results.JPG)

[Back to top](#testing)

**models.py**
* No errors found

    ![settings-warning](static/readme/testing/python-code-validation/models_results.JPG)

[Back to top](#testing)

**urls.py**
* No errors found

    ![settings-warning](static/readme/testing/python-code-validation/app_urls.JPG)

[Back to top](#testing)

**views.py**
* No errors found

    ![settings-warning](static/readme/testing/python-code-validation/views_results.JPG)

[Back to top](#testing)


</details>

- - -