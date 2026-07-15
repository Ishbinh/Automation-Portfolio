# Day 09 - API Testing with Postman

## Objective

Learn how to make HTTP GET requests using Postman, inspect JSON responses, and understand HTTP status codes.


## What I Built

- Installed and configured Postman
- Sent GET requests to public APIs
- Inspected JSON responses
- Explored GitHub REST API endpoints



## APIs Tested
GET

https://api.github.com/orgs/openai

Returned details such as:

- Login
- Name
- Description
- Repositories URL
- Blog
- Company
- Email


### Get Repository Details

GET

https://api.github.com/repos/openai/openai-python

Observed fields including:

- stargazers_count
- forks_count
- language
- open_issues_count
- default_branch



## Status Codes Observed

| Status Code | Meaning |
|-------------|---------|
| 200 OK | Request completed successfully |
| 404 Not Found | Resource or endpoint does not exist |
| API Deprecation | Learned that APIs evolve and endpoints may change over time |


## Real-world Automation Example

Monitor a GitHub repository and send an email notification when the repository reaches 100,000 stars.

Workflow idea:

Schedule Trigger
→ GitHub API
→ Check stargazers_count
→ If threshold reached
→ Send Email


## Key Takeaway

APIs are the bridge between applications. Understanding how to send requests, inspect responses, and interpret status codes is an essential skill for building reliable automations.


## Screenshots
<img width="888" height="847" alt="image" src="https://github.com/user-attachments/assets/c9c9860b-0051-429a-9d65-1bebe396321b" />
