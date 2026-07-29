# SQL Automation with Python & Email Reports

Built a small automation project that:
- Created a SQLite database for applicant data.
- Inserted sample applicant records.
- Queried the database using SQL to generate a summary.
- Formatted the query results into a report.
- Sent the report automatically via Gmail using Python SMTP.
- Stored email credentials securely using a `.env` file instead of hardcoding them.


## Files Created

### `createdb.py`
- Creates `applications.db`.
- Creates the `applicants` table.
- Inserts sample applicant records.

### `querydb.py`
- Connects to the database.
- Executes a SQL query.
- Prints the applicant summary.

### `email_report.py`
- Reads the database.
- Generates a report from SQL results.
- Sends the report as an email using Gmail SMTP.

### `.env`
Stores sensitive credentials securely.


## SQL Query Used

```sql
SELECT role,
COUNT(*) AS total
FROM applicants
GROUP BY role;
```

Output:

```
AWS: 1
DevOps: 1
```

---

## Concepts Learned

### SQLite
- Creating a local database.
- Creating tables.
- Inserting records.
- Querying data.
- Using `GROUP BY` for summaries.


### Security Best Practices
- Store credentials inside `.env`.
- Read credentials using `python-dotenv`.
- Never hardcode passwords.
- Ignore `.env` using `.gitignore`.

---

## Workflow

```
Create Database
       
        ↓

Insert Applicant Data
       
        ↓
        

Run SQL Query
        
        ↓

Fetch Results
        
        ↓

Generate Report
      
        ↓

Connect Gmail SMTP
       
        ↓

Send Email
```


## Screenshot

Successfully executed the automation:

- Database queried successfully.
- SQL summary generated.
- Email report sent successfully.

<img width="1351" height="862" alt="image" src="https://github.com/user-attachments/assets/86bffa93-608b-4d23-8541-a5885572c9ae" />


