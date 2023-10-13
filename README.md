# API Name
JSON POST with Database Integration


## API
An API endpoint that will insert and extract data in the database using POST method. 

This API uses POST method that provides more security to your endpoint rather than using Get Method that exposes your endpoint which is not advisable to use in protecting the data.
This API features the data insertion, deletion, update and print using JSON format incased within the request body making it a  light-weight data trans


## API
Endpoints

http://127.0.0.1/api/public/postName
Function:
  Inserts data into the Database.
Parameters:
  [fname, lname]

http://127.0.0.1/api/public/postUpdate
Function:
  Updates the existing data within the Database.
Parameters:
  [id, lname, fname]

http://127.0.0.1/api/public/postDelete
Function:
  Deletes the data within the Database.
Parameters:
  [id]

http://127.0.0.1/api/public/postPrint
Function: 
  Displays the data recorded inside the Database.
Parameters:
  [none]


## Request
Payloads

JSON postName Request Payload:
{
  "lname":"hortizuela",
   "fname":"manny"
}

JSON updateName Request Payload:
{
  "id":1,
  "lname":"wick",
   "fname":"john"
}

JSON deleteName Request Payload:
{
  "id":1
}

JSON printName Request Payload:
{
  "lname":"hortizuela",
   "fname":"manny"
}


## Response

JSON postName Response Payload:
{
         "status":"success","data":null
}

JSON updateName Response Payload:
{
         "status":"success","data":null
}

JSON deleteName Response Payload:
{
         "status":"success","data":null
}

JSON postPrint Response Payload:
{
         "status":"success","data":["lname":"hortizuela","fname":"manny","lname":"licayan","fname":"arnold"]
}


## Usage

To use the provided API endpoints for inserting, updating, deleting, and printing data from the database using Postman, follow these steps:

Step 1:
Open Postman:
Make sure that you have Postman installed and open it.

Step 2:
Send a POST Request to Insert Data:
For inserting data into the database using the /api/public/postName endpoint:
Set the HTTP method to POST. Enter the URL: http://127.0.0.1/api/public/postName.
In the request body, provide the parameters fname and lname with the values you want to insert into the database.
Click the "Send" button to send the request.

Step 3:
Send a POST Request to Update Data:
For updating existing data in the database using the /api/public/postUpdate endpoint:

Set the HTTP method to POST. Enter the URL: http://127.0.0.1/api/public/postUpdate.
In the request body, provide the parameters id, fname, and lname with the values you want to update in the database.
Click the "Send" button to send the request.

Step 4:
Send a POST Request to Delete Data:
For deleting data from the database using the /api/public/postDelete endpoint:

Set the HTTP method to POST. Enter the URL: http://127.0.0.1/api/public/postDelete.
In the request body, provide the parameter id with the ID of the data you want to delete.
Click the "Send" button to send the request.

Step 5: 
Send a POST Request to Print Data:
For displaying data from the database using the /api/public/postPrint endpoint:

Set the HTTP method to POST. Enter the URL: http://127.0.0.1/api/public/postPrint.
Leave the request body empty since it doesn't require any parameters.
Click the "Send" button to send the request.


## License


## Contributors
Sir. Manny R. Hortizuela
 

## Contact
Information

Email: javebrevin.torres_2@student.dmmmsu.edu.ph
Mobile #: 09384552602
