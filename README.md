# flask-blog

This is a work in progress. It is a very simple blog built with flask. The end goal is to have a blog that supports multiple authors and basic search and filter operations.

## Setup

- Create a virtualenv
- Run `pip install -r requirements.txt`
- Create a file in the top directory named `config.py`
    - You must set `SQLALCHEMY_DATABASE_URI` and `SECRET_KEY`, any other settings are optional
- Activate and start your virtualenv and run the `create_db_default_user` located in `blog/models`
- Start the development server with `python run.py`
- Now you can log in with the username and password `admin` at `localhost:5000/login/`
- Visit `localhost:5000/admin/`
    - Create a new user for yourself
    - Switch users
    - Remove the default user
    - Now start creating posts, users, tags, and services