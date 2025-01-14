# Pixly

Pixly is a RESTful API to upload, edit, and browse image files.

# Table of Contents
1. [Features](#Features)
2. [Tech stack](#Tech-stack)
3. [Install](#Install)
4. [Future features](#Future-features)

## Features<a name="Features"></a>:
* Utilizes RESTful API
* JPEG storage
* Image gallery
* Light image editing

## Tech stack<a name="Tech-stack"></a>:

### Backend:
![alt text](https://img.shields.io/badge/-Flask-000000?logo=flask&logoColor=white&style=for-the-badge)
![alt text](https://img.shields.io/badge/-Python-3776AB?logo=python&logoColor=white&style=for-the-badge)

### Database Management:
![alt text](https://img.shields.io/badge/-PostgresSQL-4169E1?logo=postgresql&logoColor=white&style=for-the-badge)
![alt text](https://img.shields.io/badge/-SQLAlchemy-F40D12?logo=sqlalchemy&logoColor=white&style=for-the-badge)

## Install<a name="Install"></a>:
Create Python virtual environment and activate:

    python3 -m venv venv
    source venv/bin/activate

Install dependences from requirements.txt:

    pip install -r requirements.txt

Setup the database:

    createdb pixly
    python seed.py

Create an .env file to hold configurations:

    SECRET_KEY=abc123
    DATABASE_URL=postgresql:///pixly

    (optional)

    AWS_BUCKET_NAME=INSERT_AWS_BUCKET_NAME
    AWS_ACCESS_KEY=INSERT_YOUR_AWS_KEY
    AWS_ACCESS_SECRET=INSERT_ACCESS_SECRET

Start the server:

    flask run

    note: on new Macs, you may have background services running on the default port 500. If so, run:

    flask run-p 5001

## Future features<a name="Future-features"></a>:
* Live image search
* Expanded image editing features
* Versioning - retrieve previous image versions.

