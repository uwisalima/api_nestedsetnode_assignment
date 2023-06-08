## Introduction
This project is a RESTful API for managing categories in an online store. The API is implemented using Laravel's nested set model and stores data in a MySQL database. The API responses are in XML format.

## Requirements
MySQL database named "online_store" with the following table:
"categories" table with columns: id, name, lft, rgt, created_at, updated_at
Laravel 10.x
PHP 8.2
## Installation
Clone the repository:
Code snippet
<code>git clone https://github.com/uwisalima/api_nestedsetnode_assignment.git</code>
Use code with caution. Learn more
Install the dependencies:
Code snippet
<code>composer install</code>
Use code with caution. Learn more
Create a MySQL database named "online_store" and run the migrations:
Code snippet
<code>php artisan migrate</code>
Use code with caution. Learn more
Usage
The API can be accessed using the following endpoints:

GET /categories: Retrieve all categories in XML format.
GET /categories/{id}: Retrieve a specific category by its ID in XML format.
POST /categories: Create a new category. Accept XML request payload with name and parent_id fields. Return the created category in XML format.
PUT /categories/{id}: Update an existing category by its ID. Accept XML request payload with name field. Return the updated category in XML format.
DELETE /categories/{id}: Delete a category by its ID. Return a success message in XML format.
Error handling and validation
The API handles errors gracefully and returns appropriate error messages in XML format. The API also validates all requests before processing them.

## Sample data
The API comes with some sample data that can be used to test the API. The sample data can be found in the database/seeders/CategorySeeder.php file.

## Unit tests
The API has been unit tested using Laravel's built-in testing framework. The unit tests can be found in the tests/Feature/CategoryTest.php file.

## Deployment
The API can be deployed to a production server using a variety of methods. One popular method is to use Laravel's built-in deployment tool, Forge. Forge makes it easy to deploy Laravel applications to a variety of hosting providers.

## Conclusion
This project has demonstrated how to create a RESTful API for managing categories in an online store using Laravel's nested set model. The API is implemented using Laravel's routing, controllers, and models. The API responses are in XML format. The API handles errors gracefully and returns appropriate error messages in XML format. The API also validates all requests before processing them. The API comes with some sample data that can be used to test the API. The API has been unit tested using Laravel's built-in testing framework.