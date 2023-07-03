# Event Driven Applications

## Event Driven Programming

### 1.What native Node.js module allows us to get started with Event Driven Programming?

It's the EventEmitter

### 2.What is the value of Object Oriented Programming used in tandem with Event Driven Programming?

This is where we can make use of Event-driven programming. By registering event listeners we can actually reverse the flow of communication between our objects. Rather than on object needing to reach inside another object to trigger a function, our objects can just emit events and whichever objects are listening to those event will process it in the way they have been told to. The source of an objects behavior is now entirely contained within itself, rather than needing to be accessed by external objects.

### 3.Consider your knowledge of Event Driven Programming in the Web Browser, now explain to a non-technical friend how Event Driven Programming might be useful on the backend using Node.js.

Every time you interact with a webpage through it’s user interface, an event is happening. When you click a button a click event is triggered. When you press a key a keydown event is triggered. These events have associated functions that, when triggered, are executed to make a change to the user interface in some way. Now imagine that you have a social media application, when someone post anything or enteract with another one that will trigger an event in the server which will send notification to others for example.
