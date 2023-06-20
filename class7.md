# Bearer Authorization

## Intro to JWT

### 1.What is a JSON Web Token (JWT)?

JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object.

### 2.When should we use JSON Web Tokens?

Authorization: This is the most common scenario for using JWT. Once the user is logged in, each subsequent request will include the JWT, allowing the user to access routes, services, and resources that are permitted with that token. Single Sign On is a feature that widely uses JWT nowadays, because of its small overhead and its ability to be easily used across different domains.

Information Exchange: JSON Web Tokens are a good way of securely transmitting information between parties. Because JWTs can be signed—for example, using public/private key pairs—you can be sure the senders are who they say they are. Additionally, as the signature is calculated using the header and the payload, you can also verify that the content hasn't been tampered with.

### 3.Claims are expected in which structural component of a JWT?

the payload

## Are JWTs Secure?

### 1.If I get a JWT and I can decode the payload, how can we call that secure?

JWTs can be either signed, encrypted or both. If a token is signed, but not encrypted, everyone can read its contents, but when you don't know the private key, you can't change it. Otherwise, the receiver will notice that the signature won't match anymore.

### 2.If sending a JWT, what must sender and receiver both know? Hint, it’s appended in the signature.

the secret

### 3.Explain how concatenated content and secret can be sent and received securely to a non-technical recruiter.

Let's assume Alice wants to send a JWT to Bob. They both know some shared secret. Mallory doesn't know that secret, but wants to interfere and change the JWT. To prevent that, Alice calculates Hash(payload + secret) and appends this as signature.

When receiving the message, Bob can also calculate Hash(payload + secret) to check whether the signature matches. If however, Mallory changes something in the content, she isn't able to calculate the matching signature (which would be Hash(newContent + secret)). She doesn't know the secret and has no way of finding it out. This means if she changes something, the signature won't match anymore, and Bob will simply not accept the JWT anymore.

## JWTs Explained

### 1.Why use JWT?

we can securely transfer information between two bodies and it's digitally signed, meaning its verified and trusted.

### 2.JWT is Compact and self-contained. Describe how this is useful to a non-technical friend.

compact meaning that it can be sent via url or using other HTTP methods and is fast, self-contained meaning it self contain all of the information from the user and we dont need to call the database more than once, we can just check if the token matches the one in store or not.

### 3.What are the three components (the structure) of a JWT signature?

base64 header with base64 payload with a secret.