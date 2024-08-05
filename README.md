This repository contains my final project for the Programmer's Assistant accreditation. 

The final project is testing an API (Application Programming Interface) via the Postman application.

Site used for testing: https://www.automationexercise.com/#google_vignette
API List of the site used for testing: https://www.automationexercise.com/api_list

Performed tests:

1. GET All Products - HTTP Response code 200 OK, which means that request was done successfully, returning the product list.
This request it is composed from request method, which defines the type of action that we wish to take it, in this case being GET, the request URL, which is like the endpoint address which we wish to interact with it, in this case being https://automationexercise.com/api/productsList, headers which offers additional information about the request, like common headers, which includes things like Content-Type, which specifies the data format that was sent and Authorization, which it can contain authentification details, request body where we include the data which we want to send to the server, in this case the list of all products, and the query parameters which contain additional information that we put on the URL. In the response body we see that we got the list of all products as result. Also I made the following JavaScript tests:
   -Response status code is 200
   -Response time is less than 1000ms
   -Validate the structure of the products array
   -Usertype and category fields within category object ar enot empty strings
   -Verify that responseCode is present and is of type number
   ![image](https://github.com/user-attachments/assets/4d62fd09-81d8-4569-857d-169ebb0b250a)
   ![image](https://github.com/user-attachments/assets/684f56f8-ba8b-4aff-b7b5-ceec5e3cfe09)

2. POST Products List – HTTP Response code 405 "This request method is not supported.", which means that the request wasn't done successfully because we tried to use a HTTP method which was unsupported by the server.
This request it is composed from request method, which defines the type of action that we wish to take it, in this case being POST, the request URL, which is like the endpoint address which we wish to interact with it, in this case being https://automationexercise.com/api/productsList, headers which offers additional information about the request, like common headers, which includes things like Content-Type, which specifies the data format that was sent and Authorization, which it can contain authentification details, request body where we include the data which we want to send to the server, and the query parameters which contain additional information that we put on the URL. In the response body we see that we got 405 response status code of This request method is not supported as result. Also I made the following JavaScript tests:
   -Response status code is 200
   -Response time is within an acceptable range
   -Response has the correct Content-Type header
   -Validate the HTML schema of the response
   ![image](https://github.com/user-attachments/assets/8f98b78c-0d06-4949-8219-6b3f4ded7e70)
   ![image](https://github.com/user-attachments/assets/02b7cfc4-0fe9-4a86-b52e-9d4e9f342338)
   
3. PUT All Brands – HTTP Response code 405 "This request method is not supported.", which means that the request wasn't done successfully because we tried to use a HTTP method which was unsupported by the server.
This request it is composed from request method, which defines the type of action that we wish to take it, in this case being PUT, the request URL, which is like the endpoint address which we wish to interact with it, in this case being https://automationexercise.com/api/brandsList, headers which offers additional information about the request, like common headers, which includes things like Content-Type, which specifies the data format that was sent and Authorization, which it can contain authentification details, request body where we include the data which we want to send to the server and the query parameters which contain additional information that we put on the URL. In the response body we see that we got 405 response status code of This request method is not supported as result. Also I made the following JavaScript tests:
   -Response status code is 200
   ![image](https://github.com/user-attachments/assets/434fb73a-4e05-4ed0-a388-b9972488ac0b)
   ![image](https://github.com/user-attachments/assets/d2cd0423-9e24-43c9-acfb-fca3436457f5)

4. GET All Brands List – HTTP Response code 200 OK, which means that request was done successfully, returning the all brands list.
This request it is composed from request method, which defines the type of action that we wish to take it, in this case being GET, the request URL, which is like the endpoint address which we wish to interact with it, in this case being https://automationexercise.com/api/brandsList, headers which offers additional information about the request, like common headers, which includes things like Content-Type, which specifies the data format that was sent and Authorization, which it can contain authentification details, request body where we include the data which we want to send to the server, in this case the list of all brands, and the query parameters which contain additional information that we put on the URL. In the response body we see that we got the list of all brands as result. Also I made the following JavaScript tests:
   -Response status code is 200
   -Response time is less than 1000ms
   -Presence of responseCode and brands fields
   -Id and brand are present in each object within the brands array
   -Id is a non-negative integer and brand is a non-empty string.
   ![image](https://github.com/user-attachments/assets/3cca2cf4-47ef-4721-98c7-954def8c139a)
   ![image](https://github.com/user-attachments/assets/32b358ed-a3af-4b98-9ec0-436d3c92d36e)
   
5. POST to Search Product – HTTP Response code 400 "Bad request, name parameter is missing in POST request.", which means that the request wasn't done successfully because the server didn't understand the request due to bad syntax.
This request it is composed from request method, which defines the type of action that we wish to take it, in this case being POST, the request URL, which is like the endpoint address which we wish to interact with it, in this case being https://automationexercise.com/api/searchProduct?search_product=top, headers which offers additional information about the request, like common headers, which includes things like Content-Type, which specifies the data format that was sent and Authorization, which it can contain authentification details, request body where we include the data which we want to send to the server and the query parameters which contain additional information that we put on the URL. In the response body we see that we got 400 response status code of Bad request, search_product parameter is missing in POST request as result. Also as parameter we put the search_product key with the "top" value. Also I made the following JavaScript test:
   -Status code is 200
   ![image](https://github.com/user-attachments/assets/c3c34ae7-5737-4382-b8f3-9eee3aae8ab0)
   ![image](https://github.com/user-attachments/assets/2c276a28-c615-432f-9e8a-2f5317941a2f)

6. POST to Search Product without search_product parameter – HTTP Response code 400 "Bad request, name parameter is missing in POST request.", which means that the request wasn't done successfully because the server didn't understand the request due to bad syntax.
This request it is composed from request method, which defines the type of action that we wish to take it, in this case being POST, the request URL, which is like the endpoint address which we wish to interact with it, in this case being https://automationexercise.com/api/searchProduct, headers which offers additional information about the request, like common headers, which includes things like Content-Type, which specifies the data format that was sent and Authorization, which it can contain authentification details, request body where we include the data which we want to send to the server and the query parameters which contain additional information that we put on the URL. In the response body we see that we got 400 response status code of Bad request, search_product parameter is missing in POST request as result. Also I made the following JavaScript test:
   -Status code is 200
   ![image](https://github.com/user-attachments/assets/9c875db7-2fee-4a26-8f0b-5b90e58b25f9)
   ![image](https://github.com/user-attachments/assets/20a32396-4f7e-44e0-9ae0-42ef97468825)

7. POST to Verify Login without e-mail parameter – HTTP Response code 400 "Bad request, name parameter is missing in POST request.", which means that the request wasn't done successfully because the server didn't understand the request due to bad syntax.
This request it is composed from request method, which defines the type of action that we wish to take it, in this case being POST, the request URL, which is like the endpoint address which we wish to interact with it, in this case being https://automationexercise.com/api/verifyLogin?password=password, headers which offers additional information about the request, like common headers, which includes things like Content-Type, which specifies the data format that was sent and Authorization, which it can contain authentification details, request body where we include the data which we want to send to the server and the query parameters which contain additional information that we put on the URL. In the response body we see that we got 400 response status code of Bad request, email or password parameter is missing in POST request as result. Also as parameter we put the password key with the "password" value. Also I made the following JavaScript test:
   -Status code is 200
   ![image](https://github.com/user-attachments/assets/ea7d8e1e-b09a-4d31-bff7-26228591f167)
   ![image](https://github.com/user-attachments/assets/67eb69e0-f62f-4b9a-b1c5-02a9c11c847e)

8. DELETE To Verify Login – HTTP Response code 405 "This request method is not supported.", which means that the request wasn't done successfully because we tried to use a HTTP method which was unsupported by the server.
This request it is composed from request method, which defines the type of action that we wish to take it, in this case being DELETE, the request URL, which is like the endpoint address which we wish to interact with it, in this case being https://automationexercise.com/api/verifyLogin, headers which offers additional information about the request, like common headers, which includes things like Content-Type, which specifies the data format that was sent and Authorization, which it can contain authentification details, request body where we include the data which we want to send to the server and the query parameters which contain additional information that we put on the URL. In the response body we see that we got 405 response status code of This request method is not supported as result. Also I made the following JavaScript test:
   -Status code is 200
   ![image](https://github.com/user-attachments/assets/893dcc94-839e-4564-a8f4-e7c727e872d4)
   ![image](https://github.com/user-attachments/assets/f9f05196-f115-4024-8884-1317b97cb99e)
   
9. POST To Create and Register User Account - HTTP Response code 400 "Bad request, name parameter is missing in POST request.", which means that the request wasn't done successfully because the server didn't understand the request due to bad syntax.
This request it is composed from request method, which defines the type of action that we wish to take it, in this case being POST, the request URL, which is like the endpoint address which we wish to interact with it, in this case being https://automationexercise.com/api/createAccount?name=test&email=test@example.com&password=password&title=Mr.&birth_date=19 &birth_month=August&birth_year=2000&firstname=Tester Name&lastname=Tester Lastname&company=Test&address1=test address&address2=secondary test address&country=testcountry&zipcode=12345&state=Test State&City=Test City&mobile_number=1234567890, headers which offers additional information about the request, like common headers, which includes things like Content-Type, which specifies the data format that was sent and Authorization, which it can contain authentification details, request body where we include the data which we want to send to the server, and the query parameters which contain additional information that we put on the URL. In the response body we see that we got 400 response status code of Bad request, name parameter is missing in POST request as result. Also as parameters we put the name key with the "test" value, the email key with the "test@example.com" value, the password key with the "password" value, the title key with the "Mr." value, the birth_date key with the "19" value, the birth_month key with the "August" value, the birth_year key with the "2000" value, the firstname key with the "Tester Name" value, the lastname key with the "Tester Lastname" value, the company key with the "Test" value, the address1 key with the "test address" value, the address2 key with the "secondary test address" value, the country key with the "testcountry" value, the zipcode key with the "12345" value, the state key with the "Test State" value, the City key with the "Test City" value and the mobile_number key with the "1234567890" value. Also I made the following JavaScript test:
   -Status code is 200
   ![image](https://github.com/user-attachments/assets/1553b72b-1839-403a-8342-52559e6da025)
   ![image](https://github.com/user-attachments/assets/d021c4be-9884-439b-938a-791fb3272cbe)

11. GET User Account Detail by E-mail - HTTP Response code 200 OK, which means that request was done successfully, returning the user account details by e-mail address.
This request it is composed from request method, which defines the type of action that we wish to take it, in this case being GET, the request URL, which is like the endpoint address which we wish to interact with it, in this case being https://automationexercise.com/api/getUserDetailByEmail?email=email@example.com, headers which offers additional information about the request, like common headers, which includes things like Content-Type, which specifies the data format that was sent and Authorization, which it can contain authentification details, request body where we include the data which we want to send to the server, in this case the user account details by e-mail address, and the query parameters which contain additional information that we put on the URL. In the response body we see that we got the list of all products as result. Also as parameters we used the email key with the "email@example.com" value. Also I made the following JavaScript tests:
   -Response status code is 200
   -Response has the required fields
   -Response time is less than 1000ms
   ![image](https://github.com/user-attachments/assets/0af37b3f-ce98-4a18-a57a-a7e780e67b30)
   ![image](https://github.com/user-attachments/assets/2a0743f9-605d-48a4-9934-eb9f2d3f4360)

Also I run the collection and I got the following results at the execution report:
Summary view of the execution report:
![image](https://github.com/user-attachments/assets/424bbd17-07d7-41dc-9efd-d385962e3ab6)
![image](https://github.com/user-attachments/assets/ca9f4d66-2508-45d5-8198-8309890a3f55)
![image](https://github.com/user-attachments/assets/554ac139-8cc4-47dd-816b-6ebd19bda386)
![image](https://github.com/user-attachments/assets/a992cdce-5a60-40ca-9d15-d6c9668c9e9b)
![image](https://github.com/user-attachments/assets/848e5a79-fc6b-4aec-96ee-8c80774c4fb6)
![image](https://github.com/user-attachments/assets/f222f21a-fa9f-4c7d-8659-64a723449e55)
![image](https://github.com/user-attachments/assets/5a086f81-5616-47c0-880e-67ebbf47d76c)
![image](https://github.com/user-attachments/assets/6e314260-fa9a-415c-94b6-560a281aa314)
![image](https://github.com/user-attachments/assets/af9d6666-0463-4ed1-b258-d41b65bed126)
![image](https://github.com/user-attachments/assets/296a8076-ba13-4cfe-bc41-d97615aaacb0)
Results view of the execution report:
![image](https://github.com/user-attachments/assets/3e7ddb38-5370-4210-af75-eab5be1a54ee)
![image](https://github.com/user-attachments/assets/be350a2c-fa08-4e3e-afcb-06b1c780d78c)
![image](https://github.com/user-attachments/assets/fbb312e8-0569-4183-bdc8-ca1e41ce695d)

Also we had 3 bugs, of which 2 of them were fixed, as we can see in the screenshots from Jira.
![image](https://github.com/user-attachments/assets/17b9a6fd-bf70-44ec-95ad-95e2da7c55c0)
![image](https://github.com/user-attachments/assets/eee5ab2e-e8e0-46db-8cbe-451f0b7c5d97)
![image](https://github.com/user-attachments/assets/3c76b3cf-a057-4fad-b366-fe5b94deb959)
![image](https://github.com/user-attachments/assets/6ff5cb5c-af3e-441f-a472-d042b19dcf7f)
![image](https://github.com/user-attachments/assets/2af46d37-bdec-43d1-ad20-57ace9d504a7)

Conclusions:
10 requests were sent to the server, and we executed 25 JavaScript tests, of which only 23 of them executed without errors.
We found and reported 3 bugs, 2 of Medium priority and one of High priority, and also we fixed 2 of the reported bugs.

