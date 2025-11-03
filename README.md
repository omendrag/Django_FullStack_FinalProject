Django_FullStack_FinalProject
A FullStack Ecommerce App built with Django and React

Table of Contents

About this App

App Overview

Products List Page

Product Details Page

Product Edit Page

Add Product Page

Checkout Page

Payment Confirmation Page

Payment Successful Page

Orders Page for User

Orders Page for Admin

Address Settings Page

Address Create Page

Address Edit Page

Card Settings Page

Card Update Page

Login Page

Register Page

User Account Page

Update User Account Page

Delete User Account Page

Other Functionalities

Installation

Backend Setup

Frontend Setup

About this App

An ecommerce app where users can purchase products using Stripe for payment.
Users can browse products freely but must create an account to proceed with purchases.
Users can delete their account anytime. On deletion, all related data (account, address, and card details) are permanently removed.

The app allows creating new Stripe cards, paying with existing ones, and deleting them.
If a Stripe card is deleted, the corresponding user account is also deleted.

App Overview

Products List Page
Displays all available products on the website.

Product Details Page
Shows detailed information about the selected product — name, description, stock status, and payment options.
Admins can edit or delete products from this page.

Product Edit Page
Accessible only to admins. Allows editing product details such as image, name, description, price, and stock status.

Add Product Page
Admins can create new products by providing required details like name, image, description, price, and stock status.

Checkout Page
Displays product information, allows payment via Stripe, and lets users select or edit their address.
Users can save their card for future use.

Payment Confirmation Page
Shows total amount, selected address, and card used for the purchase.
Users can switch cards or addresses if needed.

Payment Successful Page
Displays purchase confirmation details, including the product bought and total paid amount.
Provides a link to the orders page.

Orders Page for User
Lists all user orders, including details like name, card used, date, and delivery address.

Orders Page for Admin
Displays all users’ orders.
Admins can change product delivery statuses and use the search bar to find orders by customer name, address, or product name.

Address Settings Page
Users can view, create, edit, or delete addresses.

Address Create Page
Allows users to add a new address.

Address Edit Page
Allows users to edit existing addresses.

Card Settings Page
Displays user’s card details with options to update or delete them.

Card Update Page
Allows users to update their saved card details.

Login Page
Requires registered account credentials.

Register Page
Enables new users to sign up.

User Account Page
Displays user details like name, email, and admin privileges.

Update User Account Page
Allows users to update their username, email, and reset password.

Delete User Account Page
Enables account deletion with password confirmation.

Other Functionalities

JSON Web Tokens (JWT) are used for authentication checks.

Strong security implemented during card creation and payment.

Each request is verified using JSON tokens, except for product list and details pages.

Installation

After downloading or cloning the repository, follow the steps below.

Note: You must provide your own Stripe secret and publishable API keys in Django settings to run the project.

Backend Setup

(For Linux and Windows)

Move into the backend folder through terminal and run the following commands:

python3 -m venv env        # Windows: python -m venv env
source env/bin/activate    # Windows: env\scripts\activate
pip install -r requirements.txt
python manage.py runserver

Frontend Setup

(For Linux and Windows)

Move into the frontend folder and run the following commands:

npm i
npm start


All set! Happy Coding :)
