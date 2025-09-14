# Web-Application-for-Regex-Pattern-Matching-and-Replacement
A web app that converts natural language input received from users into regex to transform CSV/Excel data. Upload a file, describe a pattern (e.g., "match phone numbers"), and apply regex-based replacements to selected columns. The app was built with Django, React, and OpenAI. Supports previewing and downloading the transformed data.


##  Features

- Upload CSV or Excel files
- Describe patterns in natural language (e.g., "match emails", "find dates")
- Converts description to regex using OpenAI GPT-3.5
- Applies replacements to selected text columns
- Preview changes before applying
- Download transformed file as CSV

---

##  Tech Stack

- **Backend**: Django + Django REST Framework
- **Frontend**: React
- **LLM**: OpenAI API (gpt-3.5-turbo)


---

##  Project Structure

project-root/
- api/ # Django app handling API logic
- backend/ # Django project configuration (settings.py, urls.py, etc.)
- frontend/ # React frontend code
- venv/ # Python virtual environment
- .env # Contains OpenAI API key
- db.sqlite3 # SQLite database file
- manage.py # Django project runner

---

**Recommended to use a virtual environment to isolate  the dependencies.**

    venv\Scripts\activate # For Windows

---

**Make sure to set the Open_API_Key in the environment file**

**Backend: Django Setup**
    python manage.py runserver 
---
**Frontend: React Setup** 
          cd frontend 
          npm start
---
## Make sure Django is running before this

## API Overview

1.  **/api/upload/**

    - Handles file upload and parsing.

2.  **/api/regex/**

    - Accepts { description: \"match phone numbers\" }**

    - Responds with regex pattern

3.  **/api/transform/**

    - Inputs: description, column, replacement, data

    - Output: Transformed data

---

## How-to directory

- Upload a file (.csv or .xlsx)

- Describe a regex pattern in natural language

- Select column + enter replacement text

- See a highlighted preview

- Download the cleaned data as .csv

---

## Built using:

- React

- Django REST Framework

- OpenAI GPT-3.5 API

---
##Demo Video Link: 
https://drive.google.com/drive/folders/1dyC9FjlCGOF7DhBg5C_ziqv8RFcgMK9s?usp=sharing




 
