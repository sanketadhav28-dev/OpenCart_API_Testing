\# OpenCart API Testing Project



\## Project Overview



This project demonstrates API testing of an OpenCart-based e-commerce application using Postman, JavaScript assertions, API chaining, Newman, Swagger/OpenAPI, and database validation.



The project covers authentication, cart operations, response validation, dynamic variable handling, and automated execution through Newman.



\## Tools \& Technologies



\- Postman

\- REST API

\- JavaScript

\- Newman

\- Swagger / OpenAPI

\- MySQL

\- phpMyAdmin

\- Git \& GitHub

\- Jenkins



\## API Workflow



The main API workflow implemented in this project is:



1\. Create Session / Generate API Token

2\. Add Product to Cart

3\. Get Cart Details

4\. Edit Cart Quantity

5\. Verify Updated Cart

6\. Delete Cart Item

7\. Verify Cart is Empty



\## API Test Coverage



\### Authentication

\- Validate HTTP status code

\- Validate success message

\- Capture API token from response

\- Pass token to subsequent requests using Bearer Authentication



\### Add Product

\- Validate status code

\- Validate success message

\- Validate product ID

\- Validate quantity



\### Get Cart

\- Validate status code

\- Validate response success

\- Validate product details

\- Capture cart key dynamically

\- Capture cart quantity dynamically



\### Edit Cart

\- Validate status code

\- Validate success message

\- Validate cart key

\- Validate updated quantity



\### Delete Cart

\- Validate status code

\- Validate delete response

\- Verify that the cart is empty after deletion



\## API Chaining



Dynamic values are passed between requests using Postman collection variables.



Examples:



\- `api\_token\_val`

\- `cart\_key`

\- `cart\_quantity`



Example:



```javascript

pm.collectionVariables.set("api\_token\_val", jsonData.api\_token);

