# Credits - Stephan Zerhusen
# Reference - https://github.com/szerhusenBC/jwt-spring-security-demo
# springjwt
Spring JWT Template Project

This sample project can be used as a plug-in to any spring-rest application to generate JWT tokens for authenticating Restful requests.

The token will be generated after validating the user details (against the H2-DB - refer pom.xml and import.sql for more info). The 
generated token will be sent as response (in this case for /login requests).


POST - /login
* allowed for all
* Should pass user credentials

GET - /hello
* allowed only for authenticated users - refer Security config file.
* token is must for the request to be processed.
