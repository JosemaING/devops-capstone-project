**As a** developer  
**I need** to implement REST API endpoints for Account management  
**So that** I can perform CRUD operations on customer accounts through a RESTful microservice  
      
### Details and Assumptions
* The Account model includes fields: id, name, email, address, phone_number (optional), date_joined
* The service follows Model-View-Controller pattern
* Must maintain 95% code coverage
* Tests should be written first (TDD approach)
* PostgreSQL is used as the database
* Flask framework is used for the REST API
* The service runs in a containerized environment

### Acceptance Criteria     
```gherkin
Given I have an Account microservice
When I send a GET request to /accounts
Then I should receive a list of all accounts with status code 200

Given I have an Account microservice
When I send a GET request to /accounts/{id} with a valid account ID
Then I should receive the account details with status code 200

Given I have an Account microservice  
When I send a PUT request to /accounts/{id} with valid account data
Then the account should be updated and return status code 200

Given I have an Account microservice
When I send a DELETE request to /accounts/{id} with a valid account ID  
Then the account should be deleted and return status code 204

Given I have an Account microservice
When I send a request with invalid data
Then I should receive an appropriate error message with status code 400
```