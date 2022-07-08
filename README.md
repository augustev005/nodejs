# nodejs
.INTRODUCTION
A simple documentation of the API is this document, made with the Node.js language.
In the following lines I will show you how to test with different methods and types of status codes.

.ENDPOINTS
The Data Quality APIs (like any other API) are based on an event-driven architecture. 
They are triggered when an event occurs. So whenever new data arrives through a connected 
application or existing data is updated, it first passes through the API (where the data quality is checked) and
then is directed to the source database. The API thus acts as a bridge between a data capture application and a data
storage source, ensuring that no data quality errors are transferred from the first endpoint to the second.
An API endpoint is a digital location exposed via the API from which the API receives requests and sends 
responses. Each endpoint is a Uniform Resource Locator (URL) that provides the location of a resource on the API server.

REQUESTS-METHODS


The request method is how we distinguish the type of action we are "asking" our endpoint to perform.
For example, the GET method stands on its own. But we also have a few other methods that we use quite often. such as Post put ... .

Method	Description
GET	Used to retrieve information about a player.
POST	Used when inserting in the database a new data, for example the name and information of a new footballer
PUT	Used to replace an entire element (all fields) with new data. For example, changing the age or number of wins (etc ...) of a player
DELETE	Used to delete an item.
Examples

Now that we have learned the different query methods to use, we will give some examples:

Method	URL	Description

GET	/api/v1/stats/id	Retrieve all information from the player with the selected id.
POST	/api/v1/stats	Create a new post.
PUT	/api/v1/stats/id	edit post id.
DELETE	/api/v1/stats/id	DELETE post id.
real-time_example

*GET method : 

-- get the information of the players with id = 101

https://app-nodjs.herokuapp.com



*POST method : 
{
    "id": 101,
    "wins": 10,
    "losses": 3,
    "points_scored": 7
  }

-- Create a new post with id = 101

{
    "id": 101,
    "wins": 10,
    "losses": 3,
    "points_scored": 7
  }

-- Create a new post with id = 101

https://app-nodjs.herokuapp.com


  {
    "id": 231,
    "wins": 1,
    "losses": 10,
    "points_scored": 2
  }
*PUT method : 

-- edit post with id = 231

{
    "id": 101,
    "wins": 10,
    "losses": 3,
    "points_scored": 7
  }

-- Create a new post with id = 101

{
    "id": 101,
    "wins": 10,
    "losses": 3,
    "points_scored": 7
  }

-- Create a new post with id = 101

{
    "id": 101,
    "wins": 10,
    "losses": 3,
    "points_scored": 7
  }

-- Create a new post with id = 101

{
    "id": 101,
    "wins": 10,
    "losses": 3,
    "points_scored": 7
  }

-- Create a new post with id = 101

{
    "id": 101,
    "wins": 10,
    "losses": 3,
    "points_scored": 7
  }

-- Create a new post with id = 101

https://app-nodjs.herokuapp.com


  {
    "id": 231,
    "wins": 1,
    "losses": 10,
    "points_scored": 2
  }
*PUT method : 

-- edit post with id = 231

https://app-nodjs.herokuapp.com

   "id": 145,
    "wins": 5,
    "losses": 1,
    "points_scored": 14
  }
*DELETE method : 

-- Delete a post with id = 145


Code 200 to let you know that you have indeed deleted the post 

Status Codes

the status codes and their meaning if you see them on the postman test or other test :

Code	Title	Description
200	OK	When a request was successfully processed (e.g. when using GET, PATCH, PUT or DELETE).
201	Created	Every time a record has been added to the database (e.g. when creating a new user or post).
404	Not found	When URL or entity is not found.
500	Internal server error	When an internal error has happened (e.g. when trying to add/update records in the database fails).


  {
    "id": 231,
    "wins": 1,
    "losses": 10,
    "points_scored": 2
  }
*PUT method : 

-- edit post with id = 231

https://fathomless-depths-63942.herokuapp.com/api/v1/stats/20

   "id": 145,
    "wins": 5,
    "losses": 1,
    "points_scored": 14
  }
*DELETE method : 

-- Delete a post with id = 145


Code 200 to let you know that you have indeed deleted the post 

Status Codes

the status codes and their meaning if you see them on the postman test or other test :

Code	Title	Description
200	OK	When a request was successfully processed (e.g. when using GET, PATCH, PUT or DELETE).
201	Created	Every time a record has been added to the database (e.g. when creating a new user or post).
404	Not found	When URL or entity is not found.
500	Internal server error	When an internal error has happened (e.g. when trying to add/update records in the database fails).


  {
    "id": 231,
    "wins": 1,
    "losses": 10,
    "points_scored": 2
  }
*PUT method : 

-- edit post with id = 231

https://fathomless-depths-63942.herokuapp.com/api/v1/stats/20

   "id": 145,
    "wins": 5,
    "losses": 1,
    "points_scored": 14
  }
*DELETE method : 

-- Delete a post with id = 145


Code 200 to let you know that you have indeed deleted the post 

Status Codes

the status codes and their meaning if you see them on the postman test or other test :

Code	Title	Description
200	OK	When a request was successfully processed (e.g. when using GET, PATCH, PUT or DELETE).
201	Created	Every time a record has been added to the database (e.g. when creating a new user or post).
404	Not found	When URL or entity is not found.
500	Internal server error	When an internal error has happened (e.g. when trying to add/update records in the database fails).

  {
    "id": 231,
    "wins": 1,
    "losses": 10,
    "points_scored": 2
  }
*PUT method : 

-- edit post with id = 231

https://fathomless-depths-63942.herokuapp.com/api/v1/stats/20

   "id": 145,
    "wins": 5,
    "losses": 1,
    "points_scored": 14
  }
*DELETE method : 

-- Delete a post with id = 145


Code 200 to let you know that you have indeed deleted the post 

Status Codes

the status codes and their meaning if you see them on the postman test or other test :

Code	Title	Description
200	OK	When a request was successfully processed (e.g. when using GET, PATCH, PUT or DELETE).
201	Created	Every time a record has been added to the database (e.g. when creating a new user or post).
404	Not found	When URL or entity is not found.
500	Internal server error	When an internal error has happened (e.g. when trying to add/update records in the database fails).


  {
    "id": 231,
    "wins": 1,
    "losses": 10,
    "points_scored": 2
  }
*PUT method : 

-- edit post with id = 231

https://fathomless-depths-63942.herokuapp.com/api/v1/stats/20

   "id": 145,
    "wins": 5,
    "losses": 1,
    "points_scored": 14
  }
*DELETE method : 

-- Delete a post with id = 145


Code 200 to let you know that you have indeed deleted the post 

Status Codes

the status codes and their meaning if you see them on the postman test or other test :

Code	Title	Description
200	OK	When a request was successfully processed (e.g. when using GET, PATCH, PUT or DELETE).
201	Created	Every time a record has been added to the database (e.g. when creating a new user or post).
404	Not found	When URL or entity is not found.
500	Internal server error	When an internal error has happened (e.g. when trying to add/update records in the database fails).

   "id": 145,
    "wins": 5,
    "losses": 1,
    "points_scored": 14
  }
*DELETE method : 

-- Delete a post with id = 145


Code 200 to let you know that you have indeed deleted the post 

Status Codes

the status codes and their meaning if you see them on the postman test or other test :

Code	Title	Description
200	OK	When a request was successfully processed (e.g. when using GET, PATCH, PUT or DELETE).
201	Created	Every time a record has been added to the database (e.g. when creating a new user or post).
404	Not found	When URL or entity is not found.
500	Internal server error	When an internal error has happened (e.g. when trying to add/update records in the database fails).


  {
    "id": 231,
    "wins": 1,
    "losses": 10,
    "points_scored": 2
  }
*PUT method : 

-- edit post with id = 231

https://fathomless-depths-63942.herokuapp.com/api/v1/stats/20

   "id": 145,
    "wins": 5,
    "losses": 1,
    "points_scored": 14
  }
*DELETE method : 

-- Delete a post with id = 145


Code 200 to let you know that you have indeed deleted the post 

