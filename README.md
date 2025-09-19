# Intro to Load Balancing Overview Guide

**TODO:** A brief introductory guide to six methods for accomplishing server load balancing. 

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
