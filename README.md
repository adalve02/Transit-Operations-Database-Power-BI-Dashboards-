# London Transit Ridership Web App

A full-stack web app for storing, managing and exploring London transit ridership data. Built as a group project for a graduate Data Management course (ECE 9014) at Western University.

Admins can add and manage operational data, and users can filter the data and see ridership trends on interactive charts.

![Dashboard screenshot](images/dashboard.png)

## What it does
- **Stores ridership data** in a MySQL relational database, loaded from CSV/Excel files
- **Admin tools:** secure login to insert, update and manage operational data
- **Data exploration:** filter ridership by route, date and other fields
- **Trend charts:** interactive Chart.js line charts showing how ridership changes over time
- **Login and sessions:** separate access for admins and regular users

## Tech stack
| Layer | Tools |
|---|---|
| Frontend | HTML5, CSS3 (responsive dashboard), JavaScript (ES6), Chart.js |
| Backend | Python, Flask, Flask-Login, Flask-CORS |
| Database | MySQL, CSV/Excel data import |

## What I learned
- Designing a relational database schema and writing SQL to query it
- Loading raw CSV/Excel data into a clean, structured database
- Connecting a Flask backend to MySQL and serving data to a dashboard
- Adding login, sessions and user roles to a web app
- Turning query results into charts people can read quickly

## How to run it

**1. Clone the repository**
```bash
git clone https://github.com/adalve02/Datamanagementgroup11-9014.git
cd Datamanagementgroup11-9014
```

**2. Create and activate a virtual environment**
```bash
python -m venv venv
# Windows
venv\Scripts\activate
# Mac/Linux
source venv/bin/activate
```

**3. Install dependencies**
```bash
pip install -r requirements.txt
```

**4. Set up the database**
- Create a MySQL database
- Import the schema from the provided SQL file (`schema.sql`)
- Add your MySQL username and password in `config.py`

**5. Run the app**
```bash
python app.py
```
Then open `http://127.0.0.1:5000` in your browser.

## Team
Group 11, ECE 9014 Data Management, Western University
- Ashwini Dalve
- (add teammates' names)
