# Readings: CRUD

### **In your own words, describe what each group of status code represents:**

1. 100’s = informational
2. 200’s = The request was fulfilled.
3. 300’s = redirection  
4. 400’s = bad request
5. 500’s = server error

![http status codes](https://itexamanswers.net/wp-content/uploads/2020/09/2020-09-19_214640.jpg)

### **What is a status code 202?**

* **Answer:** The HyperText Transfer Protocol (HTTP) 202 Accepted response status code indicates that the request has been accepted for processing, but the processing has not been completed; in fact, processing may not have started yet. The request might or might not eventually be acted upon, as it might be disallowed when processing actually takes place.

### **What is a status code 308?**

* **Answer:** The HyperText Transfer Protocol (HTTP) 308 Permanent Redirect redirect status response code indicates that the resource requested has been definitively moved to the URL given by the Location headers. A browser redirects to this page and search engines update their links to the resource (in 'SEO-speak', it is said that the 'link-juice' is sent to the new URL).

### **What code would you use if an update didn’t return data to a client?**

* **Answer:**  If an existing resource is modified, either the 200 (OK) or 204 (No Content) response codes SHOULD be sent to indicate successful completion of the request.

### **What code would you use if a resource used to exist but no longer does?**

* **Answer:** The HyperText Transfer Protocol (HTTP) 410 Gone client error response code indicates that access to the target resource is no longer available at the origin server and that this condition is likely to be permanent.

### **What is the ‘Forbidden’ status code?**

* **Answer:** The HTTP 403 Forbidden client error status response code indicates that the server understood the request but refuses to authorize it.

-------
# Note: the video is not working // cant solve part 2 

-------


### **resources**

recource      | links
------------- | -------------
HTTP Status Code | [Link](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)
