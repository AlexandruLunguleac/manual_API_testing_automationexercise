This repository contains my final project for the Programmer's Assistant accreditation. 

The final project is testing an API (Application Programming Interface) via the Postman application.

Site used for testing: https://www.automationexercise.com/#google_vignette

Performed tests:

1. GET Lista de produse request - HTTP Response code 200 OK, which means that request was done successfully, returning the product list.
2. POST la toată lista de produse – HTTP Response code 405 "This request method is not supported.", which means that the request wasn't done successfully because we tried to use a HTTP method which was unsupported by the server.
3. PUT la lista cu toate brand-urile – HTTP Response code 405 "This request method is not supported.", which means that the request wasn't done successfully because we tried to use a HTTP method which was unsupported by the server.
4. GET ALL BRANDS LIST– HTTP Response code 200 OK, which means that request was done successfully, returning the all brands list.
5. POST to search product – HTTP Response code 400 "Bad request, name parameter is missing in POST request.", which means that the request wasn't done successfully because the server didn't understand the request due to bad syntax.
6. POST to search product without search_product parameter – HTTP Response code 400 "Bad request, name parameter is missing in POST request.", which means that the request wasn't done successfully because the server didn't understand the request due to bad syntax.
7. POST Verify Login without e-mail parameter – HTTP Response code 400 "Bad request, name parameter is missing in POST request.", which means that the request wasn't done successfully because the server didn't understand the request due to bad syntax.
8. DELETE To Verify Login – HTTP Response code 405 "This request method is not supported.", which means that the request wasn't done successfully because we tried to use a HTTP method which was unsupported by the server.
9. POST To CREATE AND REGISTER USER ACCOUNT - HTTP Response code 400 "Bad request, name parameter is missing in POST request.", which means that the request wasn't done successfully because the server didn't understand the request due to bad syntax.
10. GET USER ACCOUNT DETAIL BY E-MAIL - HTTP Response code 200 OK, which means that request was done successfully, returning the user account details by e-mail address.



