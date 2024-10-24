
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

├── app.py # Main Flask application file ├── config.py # Configuration settings for the app ├── templates/ # HTML templates │ ├── base.html # Base template │ ├── index.html # Homepage │ ├── login.html # Login page │ ├── register.html # Registration page │ └── product_list.html # Product listing page ├── static/ # Static files (CSS, images, JS) │ ├── css/ │ ├── js/ │ └── images/ ├── models.py # SQLAlchemy models for the database ├── forms.py # Flask-WTF forms for user inputs ├── requirements.txt # Python dependencies └── README.md # Project documentation

bash
Copy code

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
