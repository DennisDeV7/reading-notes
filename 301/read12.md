# CRUD

## Status Codes

1. Describe the following status codes

    - 100's = Informational status code, tells the client that the request is received and the server is working on it.
    - 200's = Success codes, tells client that the server accepted the request
    - 300's = Redirection codes: the resource is not available
    - 400's = Client errors: usually invalid requests
    - 500's = Server errors: overwhelmed or unreachable servers 

2. What is a status code 202?\
Status code 202 means the request is accepted.
3. What is a status code 308?\
Status code 308 is a permanent redirect telling the client to use a different URL
4. What code would you use if an update didn’t return data to a client?\
Status code 204: no content
5. What code would you use if a resource used to exist but no longer does?
Status code 410: Gone
6. What is the ‘Forbidden’ status code?\
Status code 403: client does not have permission to access the source

## REST API with Node, Express, & MongoDB

1. Why do we need to pull our MongoDB database string out of our server and put it into our .env?\
This way the server can access the code but the string which contains a password will not be pushed into GitHub
2. What is middleware?\
Middleware provides common services and capabilities to applications outside of what the operating system has to offer.
3. What does app.use(express.json()) do?\
Express.json is a middleware funciton of Express that parses JSON requests.
4. What does the /:id mean in a route?\
The /:id means that the code will grab information from the database by its assigned id
5. What is the difference between PUT and PATCH?\
PUT modifies the resource where the entire resource is updated. PATCH updates part of the data with out changing the entire data set.
6. How do you make a default value in a schema?\
You can make a default value in a schema by creating a document with the "default" keyword
7. What does a 500 error status code mean?\
Error Code 500 is a generic error meaning the server ran into some kind of unexpected condition
8. What is the difference between a status 200 and a status 201?\
Status code 200 means that the server successfully received a request and sent the requested data to the client. Status code 201 means that a the server created a resource as a result of a successful request from the client.

## Class

## Things I want to know more about