# Readings: APIs

## **What does REST stand for??**

* **Answer:** Representational State Transfer.

## **REST APIs are designed around a __resources__.**

* **Answer:**
 REST APIs are designed around resources, which are any kind of object, data, or service that can be accessed by the client..

## **What is an identifer of a resource? Give an example.?**

 **Answer:**
   A resource has an identifier, which is a URI that uniquely identifies that resource. For example, the URI for a particular customer order might be:

   ```
   https://adventure-works.com/orders/1
   ```

## **What are the most common HTTP verbs?**

* **Answer:**
The most common operations are GET, POST, PUT, PATCH, and DELETE.

## **What should the URIs be based on?**

* **Answer:**resource URIs should be based on nouns (the resource) and not verbs (the operations on the resource).

    ```
    https://adventure-works.com/orders // Good

    https://adventure-works.com/create-order // Avoid
    ```

## **Give an example of a good URI?**

* **Answer:**

    ```
    https://adventure-works.com/orders // Good

    https://adventure-works.com/create-order // Avoid

    ```

## **What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?**

* **Answer:**  The more requests, the bigger the load. Therefore, try to avoid "chatty" web APIs that expose a large number of small resources. Such an API may require a client application to send multiple requests to find all of the data that it require

## **What status code does a successful GET request return?**

* **Answer:** HTTP status code 200 (OK).

## **What status code does an unsuccessful GET request return?**

* **Answer:** return 404 (Not Found).

## **What status code does a successful POST request return?**

* **Answer:** HTTP status code 201 (Created)

## **What status code does a successful DELETE request return?**

* **Answer:** HTTP status code 204

----------------------------------------------------------------------

## Things I want to know more about

how get the query parameters from the defrent http request methods.

----------------------------------------------------------------------

### resources

recource      | links
------------- | -------------
Readings: APIs   | [Link](https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design)

