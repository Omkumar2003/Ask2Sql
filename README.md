# Ask2sql

**Natural Language to SQL Engine**

Ask2sql translates natural language queries into executable SQL statements, enabling users to interact with a database using plain English. It uses a Flask backend and spaCy NLP to parse, understand, and generate SQL tailored to the database schema.

---

## 🧠 How It Works

![UML Sequence Diagram](https://raw.githubusercontent.com/Omkumar2003/Ask2Sql/main/ss.png)



## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/Omkumar2003/Ask2Sql.git
cd Ask2Sql
```
### 2. Set Up the Database
Run ```sql_scripts/sql_schema.sql``` to create tables.

Run ```sql_scripts/data_feed.sql``` to populate data.

### 3. Install Dependencies
```bash
pip install -r requirements.txt
python -m spacy download en_core_web_sm
```
### 4. Configure the Application
Edit configuration/config.json:

```json
"connection_string": "DRIVER={ODBC Driver 17 for SQL Server};SERVER=your_server;DATABASE=your_db;UID=user;PWD=pass"
```
### 5. Run the App
```bash
python -B main.py
```
Visit: http://127.0.0.1:5000/




## 💬 Example Queries
```
show all students with marks greater than 30

average marks in english subject in class 12

student with maximum marks in english subject in class 12

total marks of students in class 12 in year 2019

marks of Manoj Garg student in english subject
```

