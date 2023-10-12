# API Name
Briefdescription of your API.
The PHP CRUD (Create, Read, Update, Delete) API is a web service for performing basic CRUD operations on a MySQL database. It allows you to create, retrieve, update, and delete records in a "names" database table. The API is built using the Slim framework and supports various HTTP methods for data manipulation.

 


## API
Description
The PHP CRUD API serves the purpose of providing a basic API for managing records in a MySQL database. It is designed for educational and demonstrative purposes, helping developers understand how to build a simple CRUD API in PHP using the Slim framework.

Provide a more
detailed explanation of what your API does, its purpose, and any key features.
Create: Insert new records into the "names" database table.
Read: Retrieve records from the "names" database table.
Update: Modify existing records in the "names" database table.
Delete: Remove records from the "names" database table.
Error handling: Provides basic error handling and responses for different CRUD operations.

 


## API
Endpoints
Get Name

Endpoint: /getName/{fname}/{lname}
Method: GET
Parameters: fname (required), lname (required)
Description: Retrieves a name record from the database by concatenating fname and lname.
Insert Name

Endpoint: /postName
Method: POST
Request Payload: JSON data containing fname and lname fields.
Description: Inserts a new name record into the database.
Get All Names

Endpoint: /postPrint
Method: GET
Description: Retrieves all name records from the database.
Update Name

Endpoint: /updateName/{id}
Method: PUT
Request Payload: JSON data containing fname and lname fields.
Description: Updates an existing name record in the database based on the id parameter.
Delete Name

Endpoint: /deleteName/{id}
Method: DELETE
Description: Deletes a name record from the database based on the id parameter.


Describe the
available endpoints, their functions, and the required parameters.


 


## Request
Endpoint 1: 'postName' "lname": "Tamad", "fname": "Juan"

Endpoint 2: 'printName' This endpoint does not require a Request Payload because it prints the Response Payload, which is the database's contents in JSON format.

Endpoint 3: 'updateName' "id":1, "lname":"Dela Cruz", "fname":"Juan" note: the'id' is required because it determines which record is to be updated.

Endpoint 4: 'deleteName' "id":1 Note: The 'id' parameter is the only one required for deleting records from the database.


 


## Response
Endpoint 1: 'postName'; "status":"success"; "data":null

'printName' endpoint "status":"success","data":["lname":"villanueva","fname":"antholin","lname":"gravidez","fname":"arnold"]

'updateName' endpoint "status":"success","data":null

'deleteName' enpoint 4: "status":"success","data":null

 


## Usage
Provide code
examples or instructions on how to use your API.
Step 1: Launch XAMPP or SQLyog. Step 2: Create the database 'demo' and table 'names' with columns 'id', 'lname', and 'fname'. Step 3: Store the api folder in the folder C:// >> xampp >> htdocs Step 4: Install and open Postman Step 5: Set HTTP Method whether it is GET or POST Step 6: Enter the url For endpoint 'postName': localhost/api/public/postName For endpoint 'printName': localhost/api/public/printName For endpoint 'updateName': localhost/api/public/updateName

 


## License


Mention the
license under which your API is distributed.


 


## Contributors


List
contributors or give credit to any external libraries or resources used.


 


## Contact
Information


Include contact
information for inquiries or support.
