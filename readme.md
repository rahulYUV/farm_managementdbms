
# Farm Management System
![Farm Management System Screenshot](farmer%20system/static/images/bg.jpg)


## Project Description

The **Farm Management System** is a web-based platform designed for farmers to sell agricultural products and for buyers to purchase them online. It allows users to manage various aspects of farming operations, including product listings, purchase requests, and product quality checks via email communication. This system is built using Flask for the backend and SQL for the database management.

## Features

- **Farmer Registration & Login**: Farmers can create accounts and log in to manage their products.
- **Product Listings**: Farmers can list their agricultural products for sale.
- **Buyer Requests**: Buyers can browse listed products and send purchase requests.
- **Email Notifications**: Buyers can communicate with sellers via email to check product quality or confirm orders.
- **Admin Dashboard**: The admin can manage the overall system, review transactions, and monitor user activity.

## Technologies Used

- **Backend**: Flask (Python)
- **Frontend**: HTML, CSS, JavaScript
- **Database**: SQL (SQLite)
- **Email Service**: Flask-Mail
- **Version Control**: Git & GitHub

## Project Structure


### Description of Key Components

- **app.py**: This is the main Flask application file where the app is initialized, routes are defined, and core functionalities are handled.
- **config.py**: Stores the configuration settings such as database URI, secret keys, and other environment-specific variables.
- **templates/**: Contains all HTML templates using Jinja2. These files are used to render the frontend UI.
  - `base.html`: Base layout template for the project, extended by other templates.
  - `index.html`: The homepage of the application.
  - `login.html`: Template for user login.
  - `register.html`: Template for user registration.
  - `product_list.html`: Page displaying a list of products.
- **static/**: Contains static assets like CSS, JavaScript, and images.
  - `css/`: Stylesheets used for designing the frontend.
  - `js/`: JavaScript files for adding dynamic behavior to the web pages.
  - `images/`: Static images used in the project.
- **models.py**: Defines the SQLAlchemy models that represent the structure of your database.
- **forms.py**: Contains Flask-WTF forms used for handling and validating user input for forms such as login, registration, etc.
- **requirements.txt**: Lists all the Python dependencies required to run the application.
- **README.md**: This file provides a detailed overview of the project, including setup instructions, usage, and additional information.



## Installation

To run this project locally, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/rahulYUV/farm_managementdbms.git
   cd farm_managementdbms
   ```

2. **Set up a virtual environment:**

   ```bash
   python -m venv env
   source env/bin/activate  # On Windows: env\Scripts\activate
   ```

3. **Install the dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

4. **Set up the environment variables: Create a .env file in the root directory and set the necessary environment variables (e.g., secret key, email server credentials).**

   Initialize the database:

   ```bash
   flask db init
   flask db migrate
   flask db upgrade
   ```

5. **Run the Flask app:**

   ```bash
   flask run
   ```

6. **Open the app in your browser: Visit http://127.0.0.1:5000/ to access the Farm Management System.**

## Usage
Farmers can register on the platform, log in, and list their products for sale.
Buyers can browse the available products and place purchase requests.
Admin can monitor the platform and manage user activity.
