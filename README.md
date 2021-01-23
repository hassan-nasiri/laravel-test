### Introduction
The project contains unit tests and your goal is to make sure they all pass.

### Requirements
1. Customer table with 3 required columns:
name, phone number and address

2. Customer orders table with 3 required columns:
product name, price, shipping date

3. Create a one to many relation between customers and orders

4. Create API with the following operations:
* Get customers list
* Get a customer with related orders
* Add a new customer
* Add a new order to the existing customer
* Update a customer
* Soft delete a customer


Access to each endpoint requires authentication via an API token which can be done in the custom middleware and no need to implement the user authentication.
* Api responses should follow restful api best practices.

In case of validation errors, the API should respond with a default error list from the Laravel framework (and a 422 HTTP code). The API should be protected with a rate liming mechanism.
* Configure the throttle middleware and set the rate limit to 60 reqs/minute.
