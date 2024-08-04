This repository contains my final project for the Programmer's Assistant accreditation. 

The final project is testing an API (Application Programming Interface) via the Postman application.

Site used for testing: https://www.automationexercise.com/#google_vignette

Performed tests:

1. GET All Products - HTTP Response code 200 OK, which means that request was done successfully, returning the product list.
2. POST Products List – HTTP Response code 405 "This request method is not supported.", which means that the request wasn't done successfully because we tried to use a HTTP method which was unsupported by the server.
This request it is composed from request method, which defines the type of action that we wish to take it, in this case being GET, the request URL, which is like the endpoint address which we wish to interact with it, in this case being (https://automationexercise.com/api/productsList), headers which offers additional information about the request, like common headers, which includes things like Content-Type, which specifies the data format that was sent and Authorization, which it can contain authentification details, request body where we include the data which we want to send to the server, in this case the list of all brands, and the query parameters which contain additional information that we put on the URL. In the response body we see that we got 405 response status code of This request method is not supported as result. Also I made the following JavaScript tests:
   -Response status code is 200
   -Response time is within an acceptable range
   -Response has the correct Content-Type header
   -Validate the HTML schema of the response
   
3. PUT All Brands – HTTP Response code 405 "This request method is not supported.", which means that the request wasn't done successfully because we tried to use a HTTP method which was unsupported by the server.
4. GET All Brands List – HTTP Response code 200 OK, which means that request was done successfully, returning the all brands list.
This request it is composed from request method, which defines the type of action that we wish to take it, in this case being GET, the request URL, which is like the endpoint address which we wish to interact with it, in this case being https://automationexercise.com/api/brandsList, headers which offers additional information about the request, like common headers, which includes things like Content-Type, which specifies the data format that was sent and Authorization, which it can contain authentification details, request body where we include the data which we want to send to the server, in this case the list of all brands, and the query parameters which contain additional information that we put on the URL. In the response body we see that we got the list of all brands as result. Also I made the following JavaScript tests:
   -Response status code is 200
   -Response time is less than 1000ms
   -Presence of responseCode and brands fields
   -Id and brand are present in each object within the brands array
   -Id is a non-negative integer and brand is a non-empty string.
   
5. POST to Search Product – HTTP Response code 400 "Bad request, name parameter is missing in POST request.", which means that the request wasn't done successfully because the server didn't understand the request due to bad syntax.
6. POST to Search Product without search_product parameter – HTTP Response code 400 "Bad request, name parameter is missing in POST request.", which means that the request wasn't done successfully because the server didn't understand the request due to bad syntax.
7. POST to Verify Login without e-mail parameter – HTTP Response code 400 "Bad request, name parameter is missing in POST request.", which means that the request wasn't done successfully because the server didn't understand the request due to bad syntax.
8. DELETE To Verify Login – HTTP Response code 405 "This request method is not supported.", which means that the request wasn't done successfully because we tried to use a HTTP method which was unsupported by the server.
9. POST To Create and Register User Account - HTTP Response code 400 "Bad request, name parameter is missing in POST request.", which means that the request wasn't done successfully because the server didn't understand the request due to bad syntax.
10. GET User Account Detail by E-mail - HTTP Response code 200 OK, which means that request was done successfully, returning the user account details by e-mail address.




