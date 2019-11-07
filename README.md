# JWT-Project
Src: JWT Overview https://www.youtube.com/watch?v=7Q17ubqLfaM
## What is JSON Web Token
JSON Web Tokens are an open, industry standard RFC 7519 method for representing claims securely between two parties.  
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
- A better Authorization vs session based authorization
- Authorization: Make sure its the same user that logged in.... (Different from Authentication)

## Session based  Conventional Approach) vs Token Based 
Src: https://medium.com/@sherryhsu/session-vs-token-based-authentication-11a6c5ac45e4

### Session based authentication
In the session based authentication, the server will create a session for the user after the user logs in. The session id is then stored on a cookie on the user’s browser. While the user stays logged in, the cookie would be sent along with every subsequent request. The server can then compare the session id stored on the cookie against the session information stored in the memory to verify user’s identity and sends response with the corresponding state!

![images](https://github.com/KennySoh/JWT-Project/blob/master/pic/auth1.png)

### Token Based Authentication
Many web applications use JSON Web Token (JWT) instead of sessions for authentication. In the token based application, the server creates JWT with a secret and sends the JWT to the client. The client stores the JWT (usually in local storage) and includes JWT in the header with every request. The server would then validate the JWT with every request from the client and sends response.

![images](https://github.com/KennySoh/JWT-Project/blob/master/pic/auth2.png)

### Whats a cookie
Src: https://www.youtube.com/watch?v=xdH9zsW1CK0
Src: https://www.youtube.com/watch?v=I01XMRo2ESg

Cookie is a small piece of data stored in the browser for website. Commonly used for temporary information. Similar to a dog tag, eg user.id=12345. NOrmally <4kb... (practically just 100 bytes)
  
![images](https://github.com/KennySoh/JWT-Project/blob/master/pic/cookie1.png)  
Allow google-ads network to keep track of ur online activity. 




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



