# Intro to Load Balancing Overview Guide

**Description/Overview:** Load balancing types/techniques (each corresponding to a particular kind of load balancing algorithm) are methods utilized by networks to distribute incoming data requests (traffic) from client/host devices to servers (and, possibly, server clusters). Decision to implement a specific type is based on factors such as: the nature of the app being served, what sort of service is being offered to clients, and measurements of capacity and performance of servers.

#### Table of Contents

1. [Six Load Balancing Methods](#sixmethods)
2. [Supplemental Resources](#supplemental)

<hr />

## 1. <a name="sixmethods">Six Load Balancing Methods</a>

Six popular methods for load balancing server traffic burden to avoid Single Point of Failure (SPF), other causes of server shutdown, and/or bottlenecks include:

* **Round Robin:** A load balancer forwards the data request based on sequenced order.
  + Traffic is intended for even routing distribution among servers.
* **Weighted Round Robin:** A load balancer forwards the data request based on server capacity.
* **Least Connection:** A load balancer forwards the data request to the particular server that has the fewest connections.
  + Routing distribution of traffic is dependent upon how busy the servers are.
* **Response Time:** A load balancer forwards the data request to the server that responses most quickly.
* **Source IP Hash:** A load balancer bases where it forwards the data request on the client device's IP address.
* **Resource-Based (Adaptive):** A load balancer forwards the data request based on the server's health and application performance.

<hr />

## 2. <a name="supplemental">Supplemental Resources</a>

* *[What is Load Balancing? (Cloudflare Article)](https://www.cloudflare.com/learning/performance/what-is-load-balancing/)*
* *[Amazon AWS 'What is Load Balancing? Article](https://aws.amazon.com/what-is/load-balancing/)*
* *[Wikipedia Article on Load Balancing](https://en.wikipedia.org/wiki/Load_balancing_(computing))*
