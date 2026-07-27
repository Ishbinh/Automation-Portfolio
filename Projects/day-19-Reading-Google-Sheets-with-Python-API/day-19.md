Reading Google Sheets with Python API

## Objective

Built a Python script to read data from a Google Sheet using the Google Sheets API and generate a simple summary.



## Workflow

Google Sheet


Google Sheets API


Python Script


Read Records


Generate Summary



## Technologies Used

- Python
- Google Sheets API
- Google Cloud Platform
- Service Account
- gspread
- google-auth


## Workflow Explanation

### 1. Google Cloud Setup

- Created a Service Account
- Downloaded the Service Account JSON key
- Enabled the Google Sheets API
- Shared the Google Sheet with the Service Account email


### 2. Authentication

Authenticated the Python script using the Service Account credentials.


### 3. Reading Data

Connected to the Google Sheet using its Spreadsheet ID and retrieved all records.


### 4. Processing Data

Processed the retrieved records and generated a simple summary including:

- Total number of candidates
- Candidate details
- Basic data processing using Python

