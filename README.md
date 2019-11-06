# JWT-Project
## What is JSON Web Token
***
- Open Standard
- Securely transfer information between any 2 bodies
- Digitally Signed- Information is verified and trusted
- Compact
  - JWT can be send via URL, POST request, HTTP Header
  - Fast Transimission
- Self-contained
  - Contains information about the user
  - Avoiding query the database more than once
***

## Why is JTW useful
- Authetication
- Information Exchange

## What is the JSON Web Token structure
***
- Header,
  {  
    "alg":"H256",  
    "typ":"JWT"  
  }  
  -This JSON is Base64Url encoded to form first part
- Payload
  - claims, are user details or additional metadata
  - payload is then Base64Url encoded to form the second part
- Signature
  - HMACSHA256(
      base64UrlEncode(header)+"."+
      base64UrlEncode(payload),
      secret)
***

Jwt is for authirisation (Not authentication)
make sure its the same user that logged in..
normally session id-
https://medium.com/@sherryhsu/session-vs-token-based-authentication-11a6c5ac45e4
https://www.youtube.com/watch?v=7Q17ubqLfaM

