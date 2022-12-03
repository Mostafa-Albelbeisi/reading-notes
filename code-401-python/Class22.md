# Django CRUD and Forms

The **form** is defined in HTML as a collection of elements inside `<form>…</form>` tags, containing at least one input element of `type="submit"`

The **submit** input will be displayed as a button by default. This can be pressed to upload the data in all the other input elements in the form to the server (in this case, just the team_name field).


- **action**: The resource/URL where data is to be sent for processing when the form is submitted. If this is not set (or set to an empty string), then the form will be submitted back to the current page URL.

- **method**: The HTTP method used to send the data: post or get.
     * The **POST** method should always be used if the data is going to result in a change to the server's database, because it can be made more resistant to cross-site forgery request attacks.
    * The **GET** method should only be used for forms that don't change user data (for example, a search form). It is recommended for when you want to be able to bookmark or share the URL.

## Django’s role in forms:
 1. preparing and restructuring data to make it ready for rendering
 2. creating HTML forms for the data
 3. receiving and processing submitted forms and data from the client

## What are Django forms?
 **Django** provides a Form class which is used to create HTML forms. It describes a form and how it works and appears. It is similar to the ModelForm class that creates a form by using the Model, but it does not require the Model.


## Why form is used in Django?
Django handles three distinct parts of the work involved in forms: preparing and restructuring data to make it ready for rendering. creating HTML forms for the data. receiving and processing submitted forms and data from the client.

## Example to build a Form
`<form action="/your-name/" method="post">`

`<label for="your_name">Your name: </label>`

`<input id="your_name" type="text" name="your_name" value="{{ current_name }}">`


`<input type="submit" value="OK">`
`</form>`


## Django templates
A **Django template** is a text document or a Python string marked-up using the Django template language. Some constructs are recognized and interpreted by the template engine. The main ones are variables and tags. A template is rendered with a context.

## Django views
**Django views** are Python functions that takes http requests and returns http response, like HTML documents. A web page that uses Django is full of views with different tasks and missions. Views are usually put in a file called views.py located on your app's folder.
