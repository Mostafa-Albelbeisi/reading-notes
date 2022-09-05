# Status Codes Based On REST Methods

**In your own words, describe what each group of status code represents:**

**100's =**  tell the client that the header part of the request has been received.

**200's =**  tell the client that its request was accepted

**300's =**  tell the client that the resource they are requesting isn’t available at the expected location anymore

**400's =** These are the client error codes

**500's =** These are the server error codes

**What is a status code 202?** the request has been accepted for processing, but the processing has not been completed

**What is a status code 308?** the resource requested has been definitively moved to the URL given by the Location headers.

**What code would you use if an update didn't return data to a client?** 204 No Content

**What code would you use if a resource used to exist but no longer does?** 410 Gone

**What is the 'Forbidden' status code?** The HTTP 403 Forbidden response status code indicates that the server understands the request but refuses to authorize it.

# Build A REST API With Node.js, Express, & MongoDB - Quick

**Why do we need to pull our MongoDB database string out of our server and put it into our .env?**

**What is middleware?** Middleware is software that provides common services and capabilities to applications outside of what's offered by the operating system.

**What does app.use(express.json()) do?** It parses incoming JSON requests and puts the parsed data in req.

**What does the /:id mean in a route?** The Route Order ID is a unique identifier assigned to every order that is protected by Route Package Protection. This number allows us to view all the important information to report an order issue.

**What is the difference between PUT and PATCH?** PUT is a method of modifying resource where the client sends data that updates the entire resource . PATCH is a method of modifying resources where the client sends partial data that is to be updated without modifying the entire data

**How do you make a default value in a schema?** Your schemas can define default values for certain paths. If you create a new document without that path set, the default will kick in.

**What does a 500 error status code mean?**  the server encountered an unexpected condition that prevented it from fulfilling the request.

**What is the difference between a status 200 and a status 201?**Successful. The 200 status code is by far the most common returned. It means, simply, that the request was received and understood and is being processed. A 201 status code indicates that a request was successful and as a result, a resource has been created.