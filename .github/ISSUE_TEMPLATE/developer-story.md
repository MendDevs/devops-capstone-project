---
name: Developer Story
about: This template is for developping developer stories
title: ''
labels: ''
assignees: ''

---

---
name: Account Microservice APIs

about: Add REST APIs to read, update, delete, and list customer accounts in the account microservice.

**As a** developer  
**I need** to add REST APIs to read, update, delete, and list customer accounts  
**So that** other microservices can interact with the account microservice.

### Details and Assumptions
* The database model for customer accounts has already been developed.
* The Python Flask-based REST API with an endpoint to create a customer account is already implemented.

### Acceptance Criteria
```gherkin
Given a request to read a customer account
When the account exists in the database
Then return the account details in the response

Given a request to update a customer account
When valid update data is provided
Then update the account details in the database and return a success response

Given a request to delete a customer account
When the account exists in the database
Then delete the account and return a success response

Given a request to list all customer accounts
When accounts exist in the database
Then return a list of all accounts in the response
