---
title: "Event Driven System Design with Azure Functions"
---

Events are the basic building block of asyncronous processing. Now, when I say about asynchronopus processing, we first need to understand the difference between syncronous and asynchronous processing. 

Syncronous processing is usually the way applications communicate with each other over APIs where the client awaits the server to respons within the timeout limit.
Asynchronous processing is the way where the communication between the client and server happens over a message broker. The client usually writes a message/ request on a queue, and the server listens to the queue and processes each request once at a time using FIFO principle. 

Queues are a part of the design pattern "Queue based Load Levelling". Queues are often used as a buffer between a task and a service it invokes to smoothen out the intermittent heavy load that can cause the task to timeout and the service to fail. They help to minimize the impact of peaks in demand on availability and responsiveness for both the task and the service.

