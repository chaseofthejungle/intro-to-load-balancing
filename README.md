# Intro to Load Balancing Overview Guide

**Description/Overview:** Load balancing types/techniques (each corresponding to a particular kind of load balancing algorithm) are methods utilized by networks to distribute incoming data requests (traffic) from client/host devices to servers (and, possibly, server clusters). Decision to implement a specific type is based on factors such as: the nature of the app being served, what sort of service is being offered to clients, and measurements of capacity and performance of servers.

#### Table of Contents

1. [Six Load Balancing Methods](#sixmethods)
2. [Supplemental Resources](#supplemental)

<hr />

## 1. <a name="sixmethods">Six Load Balancing Methods</a>

Six popular methods for load balancing server traffic burden to avoid Single Point of Failure (SPF), other causes of server shutdown, and/or bottlenecks include:

* **Round Robin:** A load balancer forwards the client's data request to servers based on sequenced order (rotation).
  + Traffic is intended for even routing distribution among servers. This may be appropriate if servers have approximately the same bandwidth, storage, and processing power.
    - In practice: the first data request would be sent to the first server in a round robin list, the second request would be sent to the second server, the third request to the third server, etc.
  + This is considered industry-wide to be the most common and least complex load balancing method (and corresponding algorithm).
* **Weighted Round Robin:** Similar to standard round robin, but the load balancer also considers where to forward client data requests based on server capacity (higher corresponding 'weights' are assigned to servers with greater capacity).
  + Administrators can define how to specifically 'weigh' the servers (for example: how much they would like for bandwidth to be considered by the algorithm, and to what extent).
  + This may be a more appropriate solution than standard round robin when server storage, bandwidth, and processing power vary. 
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
