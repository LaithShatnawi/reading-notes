# Authentication

## Securing Passwords

### 1.Explain to a non-technical friend how you would safely hash and store a password.

Basically, we would get the password and using a certain algorithm we would encrypt the password and save it in our database encrypted so even if some hacker got access to the database we will not be able to see the literal password.

### 2.What is Bcrypt?

is an adaptive hash function based on the Blowfish symmetric block cipher cryptographic algorithm and introduces a work factor (also known as security factor), which allows you to determine how expensive the hash function will be.
It uses a technique called Key Stretching.

### 3.Why might you use something like Bcrypt?

It introduces a security factor which is used to identify the degree of encryption required. This work factor value determines how slow the hash function will be, means different work factor will generate different hash values in different time span, which makes it extremely resistant to brute force attacks.

## Basic Auth

### 1.What is Basic Authentication?

 basic access authentication is a method for an HTTP user agent (e.g. a web browser) to provide a user name and password when making a request. In basic HTTP authentication, a request contains a header field in the form of Authorization: "Basic credentials", where credentials is the Base64 encoding of ID and password joined by a single colon :.

### 2.What properties are necessary in the header of a Basic Auth request?

ID and password joined by a single colon :

### 3.How are username:password in Basic Auth encoded?

It is encoded into an octet sequence. The character set to use for this encoding is by default unspecified, as long as it is compatible with US-ASCII, but the server may suggest use of UTF-8 by sending the charset parameter.

##

### 1.Define the authentication process to a non-technical recruiter.

Authentication is the process of verifying that an individual, entity or website is whom it claims to be. Authentication in the context of web applications is commonly performed by submitting a username or ID and one or more items of private information that only a given user should know.

### 2.How should your error messaging respond (both HTTP and HTML)? Why?

Using any of the authentication mechanisms (login, password reset or password recovery), an application must respond with a generic error message regardless of whether:

The user ID or password was incorrect.
The account does not exist.
The account is locked or disabled.
The account registration feature should also be taken into consideration, and the same approach of generic error message can be applied regarding the case in which the user exists.

The objective is to prevent the creation of a discrepancy factor, allowing an attacker to mount a user enumeration action against the application.

### 3.Bookmark this link also and consider OWASP fundamentals any time you interact with authentication. Applications developed with security in mind from inception have fewer vulnerabilities throughout their lifecycle.

[authentication cheatsheet](https://cheatsheetseries.owasp.org/cheatsheets/Authentication_Cheat_Sheet.html)