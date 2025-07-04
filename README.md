# 🍕 PizzaHub - Laravel-based Pizza Ordering System

**PizzaHub** is a dynamic web-based pizza ordering application built using **Laravel (MVC)**, **Tailwind CSS**, and **MySQL**. It features a complete pizza delivery solution with modules for customers and administrators. It supports online and cash payment methods including Stripe integration.

## 🔧 Tech Stack

- **Backend**: PHP (Laravel Framework)
- **Frontend**: Tailwind CSS, Blade Templating Engine
- **Database**: MySQL
- **Package Manager**: Composer, NPM

---

## 📁 Project Structure

/app -> Application logic (models, controllers, etc.)
/bootstrap -> Application bootstrap files
/config -> Configuration files
/database -> Database factories, migrations, seeders
/public -> Publicly accessible files (entry point index.php)
/resources -> Views, assets, and language files
/routes -> Web and API route definitions
/storage -> Compiled views, logs, and other storage
/tests -> PHPUnit test cases
/vendor -> Composer dependencies (ignored in version control)

---

## 🚀 Getting Started

### 1. Clone the Repository
    - git clone https://github.com/dhrumil0406/pizzahub.git
    - cd pizzahub

### 2. Install Dependencies
    - composer install
    - npm install

### 3. Environment Setup
    - Copy the .env.example to .env and update credentials:
        cp .env.example .env

### 4. Generate Application Key
    - php artisan key:generate

### 5. Migrate and Seed Database
    - Import the pizzahub.sql file OR use Laravel migrations if available:
        php artisan migrate --seed

### 6. Build Frontend Assets
    - npm run dev   # For development
    - npm run build # For production

### 7. Start the Server
    - Server running on [http://127.0.0.1:8000]
    - Read the routes/web.php for routes


### Features ###

- User Registration/Login (Customer)

- Admin Dashboard

- Pizza Listings & Cart System

- Order Placement and Invoice Generation

- Payment via Stripe or Cash on Delivery

- Responsive UI with Tailwind CSS

- Secure routes and role-based access

### Data for Login
- Admin -- admin -> admin1234
- Users -- example@mail.com  ->  admin1234


### Dates of created of files

14/02/2025
Admin Login Completed

15/02/2025
UserSide Design

navigation bar
index page
about page
search page
viewCart page
viewPizzaList page
viewPizza Page
viewOrder Page
viewProfile Page

// paricals for viewOrder Page
orderItemModal Page
orderStatusModal Page

16/02/2025
AdminSide Design

navigation bar
login Page
index page // after login one time only
home page // display only welcome
dashnoard page // display nav and sidebar 
// all pages show on this one dashboard page
// with one request url parameter name called "page" = "pagename"

// login session manage

categoryManage page
menuManage Page
orderManage Page
// Particals for orderPage
orderItemModal Page

21/02/2025
// user side 
// particals
checkoutModal page
orderItemModal Page
orderStatusModal Page

// admin side
categoryManage page
menuManage Page
orderManage Page

// particals
orderItemModal page
orderStatusModal Page

22/02/2025
//admin side
navbar complete
contactManage Page
userManage Page
siteManage Page
admin Logout and session
index and dashboard page fix

05/03/2025
// user side
login complete with session

08/03/2025
// user side
signup complete with session store data on db

09/03/2025
// admin side
migrations -> category, pizzaitem
models -> category, pizzaitem
controller -> categoryController, pizzaitemController
public -> catimages folder
admin navbar routes changes
pages -> categoryManage, dashboard, menuManage
category insert, update, delete completed

10/03/2025
// admin side
pages -> menuManage Page, categoryManage Page
controller -> pizzaitemController, cetgoryController
pizza_item migration changes

14/03/2025
// user side
pages -> viewPizzaList, viewPizza, indexPage
user side navbar
controller -> pizzaitemController, cetgoryController

29/03/25
//user side
// changes based on validation
navbar
signup
index
viewPizzaList
viewProfile

//admin side
// changes based on validation
navbar
index
login
menuManage
categoryManage

// migrations
users_admins
categories
pizza_items

// controller
Admin
User
PizzaItem
Category

// Models
UsersAdmin
PizzaItems
Categories

02/04/25
user side home page categories filter

loader added in categories filter

item add to cart complete

after exam given changes


04/04/25
cart manage on user side without quantity update manage


06/03/25
cart manage on user side and admin side
user manage on user side and admin side
checkout show modal and checkout function in cart controller without database

09/04/25 to 13/04/25
order migration and model
orderItems migration and model
orderItems and orderStatus modal pages on user and admin side
deliveryBoyDetails and deliveryDetails migration and model
all 4 database tables work successfully