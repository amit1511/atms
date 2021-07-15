# atms

Project Name: atoms
Java version: 1.8
Spring Boot Version: 2.5.2
Find Project Source file below,
 
Extract atms.zip and import this project.
Run application as spring boot, the default tomcat server port is 8082.

An API to get a list of all the atms
API URL: 
   http://localhost:8082/api/atoms
It will fetch all the atms from provided api https://www.ing.nl/api/locator/atms/ and return well formatted JSON response
 
An API to filter the atms by city
API URL:
	http://localhost:8082/api/atms/city?city=Lichtenvoorde

city will be request param, so in input we must provide to search city.
It will fetch all the atms which have the same city as taken in input


If city is not present, then showing custom message with status 404
For example,
http://localhost:8082/api/atms/city?city=Ranchi

 If city is blank, then throwing custom error message with status 400(Bad request) 
 http://localhost:8082/api/atms/city?city=
 
 Postmen Collection is present in repository ,
 
