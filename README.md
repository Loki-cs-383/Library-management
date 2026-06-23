# Library Management System

A simple library management system built with Flask and MySQL.

## Features

- Manage books (add, edit, delete, view)
- Manage members (add, edit, delete, view)
- Issue and return books
- Track transactions and calculate fines for late returns

## Requirements

- Python 3.x
- MySQL Server
- Flask
- PyMySQL

## Setup

1. Clone or download this repository.
2. Install the required Python packages:
   ```
   pip install -r requirements.txt
   ```
3. Create a MySQL database named `library` (or update the configuration in `app.py`).
4. Run the schema.sql to create tables and insert sample data:
   ```
   mysql -u root -p library < schema.sql
   ```
   (You will be prompted for your MySQL root password)
5. Update the MySQL configuration in `app.py` if necessary (host, user, password).
6. Run the application:
   ```
   python app.py
   ```
7. Open your web browser and go to `http://localhost:5000`

## Configuration

In `app.py`, update the `db_config` dictionary with your MySQL credentials:
```python
db_config = {
    'host': 'localhost',
    'user': 'your_username',
    'password': 'your_password',
    'database': 'library',
    'cursorclass': pymysql.cursors.DictCursor
}
```

## Screenshots

*(Add screenshots here if desired)*

## License

This project is open source and available under the MIT License.