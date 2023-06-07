# Express REST API

## Review: ES6 Classes

### 1. Classes are a template for creating \_\_\_.

objects

### 2. Can a class declaration be hoisted?

No, they cannot be hoisted

### 3. How would you describe a constructor and contextual “this” to a non-technical friend?

in programming, "this" is a special keyword that refers to the current object or instance of a class. It helps differentiate between different objects and allows you to access their properties and methods. It's like a way to say "I am" or "this specific object" within the code.

## Using Express Routing

### 1.Within Express, what does routing refer to?

Routing refers to how an application’s endpoints (URIs) respond to client requests.

### 2.What is the difference between a route path and a route method?

A route method is derived from one of the HTTP methods, and is attached to an instance of the express class.
A route path is the part of the URL that specifies the location or endpoint of a resource on a web server.

### 3.When is it appropriate to add next as a parameter to a route handler and what must you do if next has been passed to your middleware as a parameter?

In certain situations, you might want to perform some operations within a route handler and then pass control to the next middleware function in the chain.
If "next" has been passed to your middleware as a parameter, it means that your middleware function is responsible for passing control to the next middleware function in the chain.

## Express Routing

### 1.What is an Express Router?

It is a mini express application without all the bells and whistles of an express application, just the routing stuff.

### 2.By what mean do we initialize express.Router() in an express server?

We will call an instance of the express.Router(), apply routes to it, and then tell our application to use those routes 
for creating our frontend routes for our application.

### 3.What do we use route middleware for?

Route middleware in Express is a way to do something before a request is processed. This could be things like checking if a user is authenticated, logging data for analytics, or anything else we’d like to do before we actually spit out information to our user.