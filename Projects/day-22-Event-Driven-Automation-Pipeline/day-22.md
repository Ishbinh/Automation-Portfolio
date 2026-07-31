## Event-Driven Automation Pipeline (Google Sheets → n8n → FastAPI → SQLite)

## Objective
Build a complete automation pipeline that automatically stores new applicant data from Google Sheets into a SQLite database using n8n and FastAPI.


## What I Built

Created an event-driven workflow where:

Google Sheets (New Row)


Google Sheets Trigger (n8n)

      
HTTP POST Request

        
FastAPI Endpoint (Python)

        
Python Data Transformation

        
SQLite Database


## Hands-on

### Google Sheets
- Used Google Sheets as the data source.
- Added applicant details (Name, Role, Experience).

### n8n Workflow
- Configured Google Sheets Trigger.
- Trigger starts automatically whenever a new row is added.
- Used an HTTP Request node to send applicant data.

### HTTP Request
Configured:
- Method: POST


### FastAPI Endpoint

Built a POST endpoint:

```python
@app.post("/applicant")
```

Receives JSON data from n8n.

Performed basic Python transformations:

Stored the transformed data into SQLite.



### SQLite

Inserted applicant information into the `applicants` table using parameterized SQL queries.

## Concepts Learned

### Event-driven Automation
Instead of manually running Python scripts, the workflow automatically executes when a new event occurs.



### HTTP POST Request

The HTTP Request node sends applicant information as JSON to FastAPI.



### FastAPI

FastAPI exposes an API endpoint that can receive incoming requests from external applications like n8n or Postman.



## Key Takeaways

- Built my first complete event-driven automation pipeline.
- Connected Google Sheets, n8n, FastAPI, and SQLite into one workflow.
- Understood how different tools communicate using HTTP APIs.
- Learned the importance of Python data transformation before database insertion.
- Gained hands-on experience with Docker networking.

<img width="1093" height="676" alt="image" src="https://github.com/user-attachments/assets/70c85a30-fc4e-4fba-8295-40605e187950" />


