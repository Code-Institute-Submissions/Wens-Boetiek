# Wens Boetiek 
Code institute MS4 project


<!-- PROJECT LOGO -->
<br />
<h3 align="center">Wens Boetiek</h3>
<p align="center">
  </a>



<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgements">Acknowledgements</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

[Wens Boetiek][product-screenshot]](https://example.com)
Wens Boetiek is a project was set out to raise money For Make a wish Nederlands. 
it is second hand online store where poeople can donate clothes and sales made or money collected through the website are given to make a wish nederlands help
fund childern and their wishes.

This project will be an ecommerce website where user can 
  
  * Can view products donated and purchase the products
  * View stories of the current wishes that would like to be reached 
  * Users should have an account with sign up and logout function 


### Built With

This project will be  mainly with using with python and django  .
* [Bootstrap](https://getbootstrap.com)
* [JQuery](https://jquery.com)
* [django][https://www.djangoproject.com/]



<!-- GETTING STARTED -->
## Getting Started
## Contents:
<br>

* UX
  * User Stories
  * Design
  * Color
  * Layout
  * Images
  * Wireframes
  * Website Layout
  
* Features
  * Existing Features
  * Features yet to be implemented
  
* Technologies Used
  * Front End
  * Back End
  
* Planning and Testing
  * Compatibility
  * Validators
  * User Testing
  * Defensive Design

* Deployment
* Credits and Acknowledgements

### User Stories:

The user of this website is essentially anyone who is looking to purchase a musical instrument or accessories, be it a professional musician to a hobbyist to a beginner from young to old.

**"As a guest/non authenticated user I would like to ------"**
  * View and navigate the site using any device.
  * Have the option to register to become an authenticated user.
  * Easily search for all products.
  * Update Cart content.
  * Delete Cart content.
  * Use a coupon to recieve a discount.
  * Purchase a product.
  * Secure payment system.
  * View ratings and reviews for products.
  
**"As an authenticated user I would like to ------"**
  * Create a user profile, where relevent personal information can be stored.
  * Rate and review product.
  
**"As a superuser I would like to ------"**
  * Create a product.
  * Update a product.
  * Edit a product.
  * Delete a product.
  * Create a coupon.
  * Have control over all apps in admin.
  
### Design:

  The overall design concept was to provide users with a slick, smooth and pleasant to look at experience, with quick clear navigation. A Bootstrapp approach was undertaken in the design, especially for mobile.
  
  **Colors:** 
This idea was orginally started on instagram and grew popular @wensboetiek 
  i wanted to keep with original colours that were set on the instagram page 

  * lemonchiffon	#FFFACD	rgb(255,250,205)
  * black used for the letter to be more clear and easy to read
      
  To compliment the yellow hues I used earth tone colours to keep simple and really keep the eyes on the product tones.
    
      
  **Font:**
    The font used is Satisfy from google fonts.
        
  **Layout:** 
     The user should be able to be comfortable with the overall layout for a better experience. Things should be easy to access and options displayed clearly.
      
  * Homepage layout is nav bar with icon to login into the account and view shopping cart on the right /left is name of site and nave to view products
    under the title of the page which is wens boetiek 2 images will placed so that you can navigate to mens or womens products  
      
  **Navigation:**
    The navbar has a dropdown on hover feature for users quick access to desired area eg shoes , pants , jackets 
    
  **Footer:**
    Footer is transparent as not to impose and features all relevent information and social icon links.
    Some jQuery is used to keep footer displayed at the bottom of page.
        
  **Products:**
    Products are clearly displayed in cards with all relevent information regarding the product.
        
  **Cart:**
    Cart page provides added products with detailed display, options to remove or update items,and easy access to keep shoppong or go to checkout.
    
  **Checkout:**
    The checkout is expected by users to feature clear easy to fill in forms and a secure payment method, with all correct price calculations and shipping information.
    On successful secure purchase, the user is given all information of purchase and a reciept email.
    
**Features for authenticated users:**
  **Profile Page:**
    Authenticated users have the option to store their shipping information details in the forms, users are also able the review and rate products.
   
**Features for superusers:**
  Superusers have access to all the appropriate CRUD operations as regards products and other users onsite, and access to the django admin for more detailed CRUD  operations.
  CRUD operations for superusers on website:
  *  Create item
  *  Edit item
  *  Delete item
  
  
**Other Design Features:**

* The navbar is responsive on small and medium size devices using a sliding nav, achieved using a mdbootstrap modal and css.
* The navbar displayed on large screens have a dropdown hover effect, achieved using css.
* The search icon is animated to open on click, saving space, especially for mobile, pure css.
* The call to action buttons have a 'ripple' effect when clicked, incorporating the blue into the complimentary orange, a material design effect achieved using css.
* The footer uses some jQuery to keep it at bottom of page.
* Icons from [FontAwesome](https://fontawesome.com/).
* The website features Toasts, alerting users of a successful or unsuccessful action: success, warning, info and error. Toasts last 3 seconds.

**Wireframes:**
* Wireframes can be found [here](https://www.figma.com/file/aDyr7uIW2tP96CK7pqWlPu/Wen-boetiek?node-id=25%3A2)

## Project Apps:

**Home App:**
* Landing page with clear navigation, search icon and call to action enter shop button in middle of screen.

**Products App:**

Search(database):
* Users can search for items by price, rating, name, category, or by a word in the products description, in order to refine their search.  Alternatively users can search using the navigation product dropdown menu.

View products:
* Users can select any product and view it's details, and choose to add it to their shopping cart.

Superusers:
* Superusers have product CRUD options through the Products app.

Reviews:
* Authenticated users can leave a review of a product and the review is displayed in reviews section in product details.
* The rating displayed is the actual calculation of the average given rating by users.

**Models:**
* Category
* Product
* Review
* Rating


**Cart App:**
* Users can see all selected products and respective information.
* Users have the option of entering a valid coupon for discount.
* Users have the option to keep shopping or proceed to checkout.

**Contexts:**
* cart_contents function: The numeric calculations for pricing are made within this function.
* contexts:

* cart_items
* total
* product_count
* delivery
* free_delivery_delta
* FREE_DELIVERY_THRESHOLD
* sub_total
* code
* discount_total
* discount_percentage
* grand_total

**Checkout App:**
* Users can see all correct price/discount calculations including shipping cost information.
* Users can feel confident of secure payment and purchase.
* Users recieve a confirmation of purchase email.

**Models:**
* Order
* OrderLineItem

**Coupons App:**
* Where the code for the website's coupon system is created which includes validation, percentage calculation and options created for the admin.

**Models:**
* Coupon

**Profiles App:**
* When a user registers to site they are given a user profile, within which they can edit name and address, also displaying a purchase history.

**Models:**
* UserProfile

**Features yet to be implemented:**
* The option for users to edit or delete their posted reviews.
* Social Account login with allauth for quick and simple registration.
* Extra personalisation of profile page including avatar options.

## Technologies Used:

**Front End Technologies**
 * [HTML](https://en.wikipedia.org/wiki/HTML)
 * [CSS](https://en.wikipedia.org/wiki/CSS)
 * [jQuery](https://jquery.com/)
 * [Bootstrap4](https://getbootstrap.com/)
 * [stripe](https://stripe.com/ie)

**Back End Technologies**
 * [Django](https://www.djangoproject.com/)
  * Django is a high-level Python Web framework that encourages rapid development and clean, pragmatic design. 
  * django-allauth: Integrated set of Django applications addressing authentication, registration, account management as well as 3rd party (social) account authentication.
  * request-oauthlib: This project provides first-class OAuth library support for Requests.
  * django-crispy-forms: django-crispy-forms provides you with a |crispy filter and {% crispy %} tag that will let you control the rendering behavior of your Django forms in a very elegant and DRY way. Have full control without writing custom form templates. All this without breaking the standard way of doing things in Django, so it plays nice with any other form application.
  
 * [Heroku](https://en.wikipedia.org/wiki/Heroku)
  * Heroku: Used for hosting app.
  * Heroku Postgres: Used as relational SQL database plugin via Heroku.
  * dj-database-url: Utilizes the 12factor inspired DATABASE_URL environment variable to configure Django apps. I.e. Enables the connection to the Postgress remote database.
  * gunicorn: A web browser for deployed browsing.
  * psychopg2-binary: Python-PostgreSQL Database Adapter. Postgres is a server-based database that runs remotely from the Django app.(SQLite is not suitable fo long term data storage.

 * AWS
  * boto3: Boto is the Amazon Web Services (AWS) SDK for Python. It enables Python developers to create, configure, and manage AWS services, such as EC2 and S3. Boto provides an easy to use, object-oriented API, as well as low-level access to AWS services.
  * django-storages: django-storages is a collection of custom storage backends for Django.

 * [Python 3.8](https://www.python.org/)
  * Python 3.8 is the back end programming language used in the building of the website.
  
  **Notable Packages:**
  * asgiref: ASGI is a standard for Python asynchronous web apps and servers to communicate with each other, and positioned as an asynchronous successor to WSGI.
  * autopep8: autopep8 automatically formats Python code to conform to the PEP 8 style guide.
  * Pillow:  Adds support for opening, manipulating, and saving many different image file formats.
  
## Testing:
 
 * Google Chrome was used as primary testing browser, also some testing on firefox and safari.

**Navigation**
 * Links tested on navbar.
 * Links tested on footer.
 * All button links tested.
 * Toasts tested.
 * Product links navigate to product detail page.
 * Update product links navigate to product detail page and update occurs.
 * Delete product links navigate to product detail page and deletion occurs.
 * Search bar finds correct search.
 
**Purchasing**
 * Add items to cart adds the correct item to cart.
 * Update the cart by reducing or increasing the quantity of any item in cart.
 * Remove cart item removes from cart.
 * add coupon codes to bag contents and have the costs updated.
 * prevent multiple coupons to be appended in order to get fraudalent discount.
 * email responses to purchases.

**Stripe Payments and Transaction Data**
 * Transactions are recorded in the Postgress db and can be accessed and selectively edited.
 * Payments are recorded on Stripe using test credit card no.
 * Stripe webhooks.

**Authentication**
 * Login and registration links work.
 * Links within allauth app e.g. password reset.
 * Email response to aunthentication.

**Toasts**
 * Toasts work when called and relevent information displays, last the set 3 seconds before dissapearing.

**Form Validation**
 * **Registration Form:**
  * Email address: input field requires an '@' character.
  * Username
  * Password

 * **Login Form:**
  * Email address: input field requires an '@' character.
  * Username.
  * Password.

 * **Password Reset Form:**
  * Email address: input field requires an '@' character.

 * **Review Form:**
  * Review posts and displays correctly.
  * Correct rating is posted and average calculated with `reviews_avg = reviews.aggregate(Avg('rate'))`

**Cart**
 * **Add item to cart:**
  * Correct item is added with all correct data.
  * Correct product price is calculated.
  * Coupon gives proper percentage discount.
  * Update gives correct resonse with toast.
  * Delete deletes product from cart.
  * Empty cart displays message "Your shopping cart is empty".

**Checkout**
 * **Add item to checkout:**
  * Item details display correctly on page.
  * Correct price including discounts is displayed.
  * Shipping form works.
  * Email Response to purchase is sent.

**Coupons:**
 * The coupon is created by a superuser in the admin, with a code, valid from to dates and a percentage option for the discount amount.
 * The created valid coupon when added subtracts the correct amount from total price, followed by a success toast.
 * Entry of an invalid code results in an error toast.

**Authenticated User Operations:**
 * Changing and saving personal details successful.
  
**Superuser CRUD Operations:**
 * Items successfully added.
 * Items successfully edited and updated.
 
**Responsiveness:**
  
  All pages rendered on website have been tested for responsiveness on a range of devices:
  * Large: Acer chromebook / windows desktop 
  * Medium: Ipad
  * Small: samsung A20s and iphone 7 
  
  Any major cross-device issues have been dealt with through media queries in css.
  
**Validators**

 * [W3C HTML Validator](https://validator.w3.org/)
  * No errors other than python such as template variables.

 * [W3C CSS Validator](https://jigsaw.w3.org/css-validator/)
  * No errors found.

 * Tested JavaScript using google chrome dev tools:
  * Toastjs: No Errors.
  * countryfieldjs: No Errors.
  * Stripejs: No Errors.
  * footerjs: No Errors.

 **Python**
  * [PEP8](http://pep8online.com/)
   * No errors found.
   * All python files worked on over the course of this project have been formatted with flake8 on vscode.

# Security/Defensive Design:
 
  * Form validation using crispy forms and required fields in the apps' models ensured that users only input acceptable data.
  
  * All forms intelligently handle empty or invalid input fields.
  
  * Any sensitive code has been hidden in files such as env, IDE settings or 3rd parties.
  
  * Different levels of site users, authenticated users, staff users and superusers gives a range of permissions for CRUD activities on the site.
  
  * Extensive testing for the site navigation was done making sure everything still works. eg: navigating back to the login page after already being logged in.
  
  * Clear feedback to the user is given for any disallowed action.
  
  * All forms are autopopulated where appropriate once users are authenticated.
  
  * The allauth authentication system has been implemented.
  
  * The filing system is uniform and standard throught the numerous apps. All apps have been tested against the standard validators for code.

## Deployment

**Local Deployment**

1. Basic requirements for deployment:
   * Python3 to run the application.
   * PIP to install app requirements.
   * An IDE (eg:gitpod)
   * GIT for cloning and version control.
   * A Github account for saving repositories.
   * Stripe account for implementing payment system.

2. 
   ```

3. Go to this folder in your IDE's terminal.
4. Enter the following command into your terminal.
   ```
   python3 -m .venv venv
   ```

5. Install the requirements and dependancies from the requirements.txt file.
   ```
   pip3 -r requirements.txt
   ```
6. Run a PostgresSQL database.
* `os.environ.setdefault('SECRET_KEY', '')`
* `os.environ.setdefault('STRIPE_PUBLIC_KEY', '')`
* `os.environ.setdefault('STRIPE_SECRET_KEY', '')`
* `os.environ.setdefault('STRIPE_WH_SECRET', '')`
* `os.environ.setdefault('EMAIL_HOST_USER', '')`
* `os.environ.setdefault('EMAIL_HOST_PASS', '')`
* `os.environ.setdefault('EMAIL_HOST_USER', '')`
* `os.environ.setdefault('AWS_ACCESS_KEY_ID', '')`
* `os.environ.setdefault('AWS_SECRET_ACCESS_KEY', '')`
* `os.environ.setdefault('DATABASE_URL', '')`

7. Add env to .gitignore file to avoid any sensitive data being pushed to github.
8. Type into terminal to migrate
```
python3 manage.py migrate
```
9. Type into terminal to run
```
python3 app.py
```

**Deployng to Heroku**
 
 * Sign up and login to Heroku.
 * Once logged in select 'create new app'.
 * Name app and select region.
 * Create app
 * In resources and add Heroku Postgres Database.
 * Go back to your IDE and install dj-database-url and psycopg2-binary.
 * Run pip3 freeze > requirements.txt.
 * Set up database by going to settings.py and import dj-database-url
 * In settings.py navigate to database settings and replace default database with a call to dj_database_url.parse().
 * Add database URL found in Heroku settings config vars.
 * Run python3 manage.py migrate .
 * If uploading data using json fixtures you can enter python3 manage.py loaddata <fixture name>.
 * Add superuser to log in with python3 manage.py createsuperuser.
 * DO NOT commit with Heroku database settings visible change database back to original database URL before commit.
 * Insall gunicorn and freeze requirements.
 * Create our Procfile that creates a web dyno in Heroku.
 * Temporarilly disable collect static by entering heroku config:set DISABLE_COLLECTSTATIC = 1 --<project name>.
 * Add Host name of heroku app to allowed settings.py, allow local host also to access from your IDE.
 * To push to heroku you may need to initialise your heroku git remote heroku git:remote -a <project name>.
 * Then push to heroku git push heroku master.
 * In Heroku app go to deploy tab and select github to link Heroku and whatever is pushed to github.
 * Enable automatic deploys.
 * Get secret key and add to heroku config settings.
 * Go to settings.py remove secret key and replace with a call to get it from the environment *SECRET_KEY = os.environ.get('SECRET_KEY', '')
 * Set debug to be True only if there is a variable called development in the environment DEBUG = 'DEVELOPMENT' in os.environ.

## Notes on Resubmission:

 Feedback from the assessment team addressed:
 
 * 1.2: X-scroll issue caused by too much margin added to nav elements making the navbar wider than the body.
   Solution: Margin reduced on nav elements making sure all elements in body are contained within.  Add to cart button added to main products page as recommended.
 
 * 1.4: Server Error (500) when negative values are added in Quantity field in the product details page.
   Solution: Javascript added that prevents negative values or blank in Quantity field in the product details page.
 
 * 1.8: Layout off grid on medium screen sizes caused by navbar larger than body.
   Solution: Reduced margin from navbar so not to overflow.
 
 * 4.1: Checkout sometimes leads to a server error when fields are incorrectly filled.
   Javascript added for defensive design preventing negative values in fields and also blank. In checkout models OrderLineItem product had size charfield max_length set to 2, checking out items with a size or string guage would lead to Server Error (500) because sizes were up to 11 characters eg: extra-light, 
 charfield max_length increased to solve this issue.
 
 * 5.4: Please refer to commits made from when I resumed project for resubmission - beginning 19th May.
   
 
 
 
## Credits

* [ckz8780](https://github.com/ckz8780/boutique_ado_v1) as the entire website is built upon the boutique ado tutorial.
* [Dennis Ivy youtube channel](https://www.youtube.com/channel/UCTZRcDjjkVajGL6wd76UnGg)
* [Mdbootstrap](https://mdbootstrap.com/) templates
* Images and data all from owner of site and authorised through make a wish and parents of the a make a wish foundations 

## Acknowledgements:

 * Code Institute tutors Jo, Cormac, Igor, Tim, Johann, Sheryl, Michael, Alan, Kevin and those whom I forgot.
 *  for mentoring support throughout the course.
 * Everyone at Code Institute for great support throughout the past year.
