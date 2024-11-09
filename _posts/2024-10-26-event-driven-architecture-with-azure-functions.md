---
title: Event Driven System Design with Azure Functions
---

Events serve as the fundamental building blocks for asynchronous processing. To understand asynchronous processing, it’s essential to first differentiate between synchronous and asynchronous approaches.

In synchronous processing, applications often communicate via APIs, where the client sends a request and waits for the server to respond within a specified timeout period. This form of processing is commonly used for real-time, immediate-response interactions.

In contrast, asynchronous processing enables communication between the client and server through a message broker. Here, the client places a request or message into a queue, and the server listens to the queue and processes each request sequentially, following the First-In, First-Out (FIFO) principle.

Queues are a key component of the "Queue-based Load Leveling" design pattern. They act as a buffer between a task and the service it invokes, helping to manage sudden surges in demand. By smoothing out spikes in workload, queues reduce the likelihood of task timeouts and service failures, thereby enhancing the availability and responsiveness of both the task and the service.