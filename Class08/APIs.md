# API Design Best Practices
**What does REST stand for?** REST is an acronym for REpresentational State Transfer and an architectural style for distributed hypermedia systems.

**REST APIs are designed around a** resources.

**What is an identifier of a resource? Give an example.** Resource identification refers to the unambiguous reporting of research resources such as genes, organisms, tools, and reagents (such as antibodies).

**What are the most common HTTP verbs?**  POST, GET, PUT, PATCH, and DELETE.

**What should the URIs be based on?** be based on nouns (the resource) and not verbs (the operations on the resource).

**Give an example of a good URI.** /orders/99/customer

**What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?** I think yes, it's so beneficial, maybe sometimes you need to contact service to help you and contact people.

**What status code does a successful GET request return?** 200 (OK)

**What status code does an unsuccessful GET request return?** return 404 (Not Found)

**What status code does a successful POST request return?** 201 (Created)

**What status code does a successful DELETE request return?** 204 (No Content)

## Things I want to know more about