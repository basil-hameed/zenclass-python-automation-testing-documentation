### Python Database Connectivity ###

---

Python provides libraries such as **sqlite3** and **PyMySQL** for database connectivity. These libraries allow Python applications to connect to databases, execute SQL queries, and retrieve results. Here's an example using **sqlite3**, which is part of Python's standard library.

---

**Example (Connecting to a SQLite Database):**
```python
import sqlite3

# Establish a connection to the database (or create one if it doesn't exist)
connection = sqlite3.connect('example.db')

# Create a cursor object to interact with the database
cursor = connection.cursor()

# Create a table
cursor.execute('''
    CREATE TABLE IF NOT EXISTS Users (
        ID INTEGER PRIMARY KEY AUTOINCREMENT,
        Name TEXT NOT NULL,
        Age INTEGER NOT NULL
    )
''')

# Insert data into the table
cursor.execute('INSERT INTO Users (Name, Age) VALUES (?, ?)', ("Alice", 30))
cursor.execute('INSERT INTO Users (Name, Age) VALUES (?, ?)', ("Bob", 25))

# Commit the changes
connection.commit()

# Query data from the table
cursor.execute('SELECT * FROM Users')
rows = cursor.fetchall()

# Print the results
for row in rows:
    print(f"ID: {row[0]}, Name: {row[1]}, Age: {row[2]}")

# Close the connection
connection.close()
```

---

**Steps Explained:**

1. **Connect to Database:**
   Use `sqlite3.connect()` for SQLite or libraries like PyMySQL for MySQL. Specify the database file or connection string.

2. **Create Cursor:**
   A cursor is used to execute SQL queries and fetch results.

3. **Execute SQL Statements:**
   - Create tables using `CREATE TABLE`.
   - Insert data with `INSERT INTO`.
   - Query data with `SELECT`.

4. **Fetch Results:**
   Use methods like `fetchone()`, `fetchmany(size)`, or `fetchall()` to retrieve query results.

5. **Commit and Close:**
   - Use `commit()` to save changes for queries like INSERT, UPDATE, DELETE.
   - Close the connection using `connection.close()`.

---

**Connecting to MySQL (using PyMySQL):**
To connect to MySQL, install PyMySQL using:
```bash
pip install pymysql
```

**Example:**
```python
import pymysql

# Database credentials
host = "localhost"
user = "your_username"
password = "your_password"
database = "ExampleDB"

# Establish connection
connection = pymysql.connect(host=host, user=user, password=password, database=database)

cursor = connection.cursor()

# Execute a query
cursor.execute("SELECT * FROM Users")

# Fetch results
rows = cursor.fetchall()
for row in rows:
    print(f"ID: {row[0]}, Name: {row[1]}, Age: {row[2]}")

# Close the connection
cursor.close()
connection.close()
```
