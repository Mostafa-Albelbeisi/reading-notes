# Django

**Django** is a back-end server side web framework. Django is free, open source and written in Python. Django makes it easier to build web pages using Python. Django is a high-level Python web framework that enables rapid development of secure and maintainable website

## Django helps you write software that is:
- Complete
- Versatile
- Secure
- Scalable
- Maintainable
- Portable

## How to install Django
`$ python -m django --version`


### Object-relational mapper:
 You get a rich, dynamic database-access API for free — but you can still write SQL if needed.

 ### URLs and views:
 To design URLs for an application, you create a Python module called a URLconf. Like a table of contents for your app, it contains a simple mapping between URL patterns and your views.

 ### Templates:
 language is designed to strike a balance between power and ease, It’s designed to feel comfortable and easy-to-learn to those used to working with HTML, like designers and front-end developers. But it is also flexible and highly extensible, allowing developers to augment the template language as needed.

 ### Forms:
 Django provides a powerful form library that handles rendering forms as HTML, validating user-submitted data, and converting that data to native Python types. Django also provides a way to generate forms from your existing models and use those forms to create and update data.

 ### Authentication:
 Django comes with a full-featured and secure authentication system. It handles user accounts, groups, permissions and cookie-based user sessions. This lets you easily build sites that allow users to create accounts and safely log in/out.

## What does Django code look like?
A web application waits for HTTP requests from the web browser When a request is received the application works out what is needed based on the URL and possibly information in **POST** data or **GET** data,  Depending on what is required it may then read or write information from a database or perform other tasks required to satisfy the request.
**Django web applications typically group the code that handles each of these steps into separate files:**
* **URLs:** While it is possible to process requests from every single URL, it is much more maintainable to write a separate view function to handle each resource
* **View:** A view is a request handler function, which receives HTTP requests and returns HTTP responses. Views access the data needed to satisfy requests via models, and delegate the formatting of the response to templates.
* **Models:** the structure of an application's data, and provide mechanisms to manage (**add**, **modify**, **delete**) and query records in the database.
* **Templates:**  is a text file defining the structure or layout of a file (such as an **HTML page**),  A view can dynamically create an HTML page using an HTML template.