# python-crud-api
## This project is a submission for Backend role at ProKhelo

This is a simple CRUD API built with Python and MySQL that allows users to log in, create their profile, edit their profile, and get all users from the API.

## Installation

1. Clone this repository
2. Create a virtual environment: `python3 -m venv venv`
3. Activate the virtual environment: `source venv/bin/activate`
4. Set up your MySQL database by running the `sql_script.sql` file in your MySQL server.
5. Update the MySQL database information in `server.py`, `login.py`, and `user_create.py` files with the appropriate information for your MySQL server.

## Usage

1. Start the server: `python server.py`
2. To log in, send a POST request to `http://localhost:5000/login` with the user's email and password in the request body.
3. To create a user profile, send a POST request to `http://localhost:5000/user/create` with the user's email, name, and age in the request body.
4. To edit a user's profile, send a PUT request to `http://localhost:5000/user/edit` with the user's email and the new name and/or age in the request body.
5. To get all users, send a GET request to `http://localhost:5000/user/all`.
