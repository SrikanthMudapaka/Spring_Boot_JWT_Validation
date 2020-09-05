# Spring_Boot_JWT_Validation
************************ Spring_Boot_JWT_User_valiation *************************************

*) Customers sign in by submitting their credentials to the provider.

*)  Upon successful authentication, it generates JWT containing user details and privileges for accessing the services and sets the JWT expiry date in payload.

*)The server signs and encrypts the JWT if necessary and sends it to the client as a response with credentials to the initial request.

*)Based on the expiration set by the server, the customer/client stores the JWT for a restricted or infinite amount of time.

*)The client sends this JWT token in the header for all subsequent requests.

*)The client authenticates the user with this token. So we don't need the client to send the user name and password to the server during each authentication process, but only once the server sends the client a JWT.
techgeeknext

first, perform post request : localhost:9090/authenticate using username and paswword as JSON object
the server would generate a JWT Token using these for access the application like performing Get request send the JWT Token in the header using Bearer.
 
 **********************IN JWT VALIDATIONS EVERY USER HAS A UNIQUE NAME ****************************
