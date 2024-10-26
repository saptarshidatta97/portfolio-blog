---
title: "Event Driven Design with Azure Functions"
categories:
  - Software Architectures
tags:
  - Software Architecture
  - Events
  - Azure Functions
---

Events arte the basic building block of asyncronous processing. Now, when I say about asynchronopus processing, we first need to understand the difference between syncronous an dasynchronous processing. 

Syncronous processing is usually the way applications communicate with each other over APIs where the client awaits the server to respons withing the timeout limit.
Asynchronous processing is the way where the communication between the client and server happens over a message broker. The client usually writes a message/ request on a queue, and the server listens to the queue and processes each request once at a time using FIFO principle. 

