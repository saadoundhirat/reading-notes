# Readings: REST

## **Who is Roy Fielding?**

* **Answer:** He helped write the first web servers, that sent documents across the internet… and then he did a ton of research explaining why the web works the way it does. His name is on the specification for the protocol that is used to get pages from servers to your browser.

Roy Thomas Fielding (born 1965) is an American computer scientist, one of the principal authors of the HTTP specification and the originator of the Representational State Transfer (REST) architectural style. He is an authority on computer network architecture and co-founded the Apache HTTP Server project.

## **Why don’t the techniques that we use today work well when we need to be able to talk to all of the machines in the world?**

* **Answer:** Because they weren't designed to be used like that. When Fielding and his colleagues started building the web, being able to talk to any machine anywhere in the world was a primary concern. But most of the techniques developers later used to get computers to talk to each other didn't have those requirements. You just needed to talk to a small group of machines.

## **What is the HTTP protocol that Fielding and his friends created?**

 **Answer:**
   HTTP—this protocol Fielding and his friends created—is all about applying verbs to nouns. For instance, when you go to a web page, the browser does an HTTP GET on the URL you typed in and back comes a web page.

## **What does a GET do?**

* **Answer:**
GET is used to request data from a specified resource.

GET is one of the most common HTTP methods.

Note that the query string (name/value pairs) is sent in the URL of a GET request:

## **What does a POST do?**

* **Answer:**
POST is used to send data to a server to create/update a resource.

The data sent to the server with POST is stored in the request body of the HTTP request:

## **What does PUT do?**

* **Answer:**
The HTTP PUT request method creates a new resource or replaces a representation of the target resource with the request payload.

The difference between PUT and POST is that PUT is idempotent: calling it once or several times successively has the same effect (that is no side effect), whereas successive identical POST requests may have additional effects, akin to placing an order several times.

## **What does PATCH do?**

* **Answer:**
The HTTP PATCH request method applies partial modifications to a resource.

PATCH is somewhat analogous to the "update" concept found in CRUD (in general, HTTP is different than CRUD, and the two should not be confused).

A PATCH request is considered a set of instructions on how to modify a resource. Contrast this with PUT; which is a complete representation of a resource.

----------------------------------------------------------------------

## Things I want to know more about

how get the query parameters from the defrent http request methods.

----------------------------------------------------------------------

### resources

recource      | links
------------- | -------------
How I explained REST to my brother   | [Link](https://gist.github.com/brookr/5977550)
Roy Fielding | [Link](https://en.wikipedia.org/wiki/Roy_Fielding)
HTTP Request Methods | [Link](https://www.w3schools.com/tags/ref_httpmethods.asp)
PUT | [Link](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods/PUT)
PATCH | [Link](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods/PATCH)
