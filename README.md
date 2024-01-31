Real Estate Website

This is a real estate website that allows landlords to create user accounts, upload property listings with images and videos, while tenants can create user accounts and browse available property listings. The application is built using HTML, CSS, and FastAPI.
Prerequisites

Before running the application, ensure you have the following installed:

    Python
    FastAPI
    SQLAlchemy
    Jinja2 Templates
    Cloudinary (for image and video storage)
    A web browser

Installation

    Clone this repository to your local machine:

    bash

git clone https://github.com/your-username/real-estate-website.git
cd real-estate-website

Create a virtual environment (optional but recommended):

bash

python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`

Install the required Python packages:

bash

pip install -r requirements.txt

Set up Cloudinary account:

    Create an account on Cloudinary.
    Obtain your Cloudinary API key and API secret.
    Update the Cloudinary configuration in the app.py file with your credentials.

Initialize the database:

bash

    alembic upgrade head

Usage

    Start the FastAPI server:

    bash

    uvicorn main:app --reload

    The application should now be running locally. You can access it by opening your web browser and navigating to http://localhost:8000.

    Landlords and tenants can sign up for user accounts through the respective registration pages.

    Landlords can log in and add property listings, including details like address, rent, number of rooms, and upload images and videos. Tenants can log in and browse available property listings.

    Users can click on a property listing to view more details and images.

    Documents uploaded by tenants can be accessed in the "Documents" section.

Features

    User registration and authentication for landlords and tenants.
    Landlords can add property listings with images and videos.
    Tenants can browse available property listings.
    Pagination for listing pages.
    Cloudinary integration for image and video storage.
    Responsive user interface with HTML and CSS.
    Document management for tenants.

Customization

    You can customize the appearance and layout of the website by modifying the HTML and CSS files in the templates directory.
    Additional features and improvements can be made by extending the FastAPI application in the app.py file.

Credits

This real estate website project utilizes the following technologies and libraries:

    FastAPI: A modern, fast (high-performance) web framework for building APIs.
    SQLAlchemy: A powerful SQL toolkit and Object-Relational Mapping (ORM) library.
    Jinja2 Templates: A template engine for Python, used for rendering HTML templates.
    Cloudinary: A cloud-based image and video management platform.
    Alembic: A database migration tool for SQLAlchemy.
    HTML and CSS for the user interface.

License

This project is licensed under the MIT License.
