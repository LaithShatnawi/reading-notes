# Readings: Express, NPM, TDD, CI/CD

Express, NPM, TDD, and CI/CD are essential elements in modern web development. They contribute to efficient development workflows, code quality, collaboration, and faster delivery of reliable web applications.

## An introduction to NodeJS and Express

### 1.Explain middleware, answer as though I were a non-technical recruiter.

a middleware is a helpful intermediary or assistant that sits between different components of a system, facilitating communication and adding extra functionality.

### 2.Express the most popular __ __ __.

framework for node js

### 3.Express is “unopinionated.” What does that mean?

It allows developers to have a lot of freedom and flexibility in how they structure their applications and handle various aspects of web development.

### 4.What is a module and why is modularity useful to us as developers?

a module refers to a self-contained and reusable unit of code that performs a specific functionality or provides a particular set of features. modularity plays a vital role in software development by enhancing reusability, maintainability, organization, collaboration, and scalability. It promotes code efficiency and clarity, allowing developers to build complex systems with ease and flexibility.

## What is NPM?

### 1.What version of npm are you running on your machine?

version 9.5.0

### 2.What command would you type to install a library/package called ‘jshint’ into your node project?

npm install jshint

## What is TDD?

### 1.Explain why tests are important. Please explain as though I were your non technical elder.

JavaScript tests act as inspectors for our software. They examine our code, verify its correctness, and identify any issues or bugs. By writing tests, we create a set of instructions that describe how our code should behave in various situations. When we run these tests, they automatically check if the code functions as intended, flags any discrepancies or errors, and gives us confidence that our code is working correctly.

### 2.What are three expected benefits of testing

Bug Identification and Prevention, Increased Confidence and Reliability, Maintenance and Scalability

### 3.Name at lest 2 individual pitfalls and at least 2 team pitfalls commonly encountered while writing tests.

Individual Pitfalls:

1.Overlooking Edge Cases
2.Writing Brittle Tests

Team Pitfalls:

1.Lack of Test Coverage
2.Neglecting Test Maintenance

## CI/CD

### 1.What are three benefits of Continuous Integration?

1.Early Detection of Integration Issues
2.Faster Feedback Loop
3.Increased Confidence and Quality Assurance

### 2.What is the difference between Continuos Delivery and Continuous Deployment?

the key difference between Continuous Delivery and Continuous Deployment lies in the deployment stage. Continuous Delivery automates and streamlines the process up to the point of making the software ready for deployment, leaving the actual deployment decision to the team. Continuous Deployment, on the other hand, takes it a step further by automating the deployment process itself, automatically pushing changes to the production environment without manual intervention.

### 3.Explain how GitHub fits into this process assuming the listener comes from a non-technical background

In the context of Continuous Integration (CI), GitHub provides a foundation for automating the process of building, testing, and integrating code changes. Developers use Git, a version control system, to manage their codebase locally. They can make changes to the code on their own machines and then use Git to push those changes to the GitHub repository. GitHub keeps track of the different versions of the code, allowing developers to collaborate, review, and merge their changes together.
