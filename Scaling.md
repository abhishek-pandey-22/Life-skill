



# Scalability

Suppose You have a set of codes that perform some task based on request and response and you want to make it available for more people. For that, you need to expose your code using some protocols which are running on the internet. But if you made it available for more clients then it might not perform well or stuck because many users are using it. So for that, you need to expand your performance criteria and that can be done using either Buying more machines or Buying bigger machines.

### Definition

The ability to handle more requests by buying more machines or buying a bigger machine is called Scalability.

### Types of Scaling

#### 1. Vertical Scaling (Buying bigger machine)
#### 2. Horizontal Scaling (Buying more machine)
![1_kJwD0kMDHx9ZjZEHeKr8yg](/uploads/60492df2820a63eff4d341fa85b3213a/1_kJwD0kMDHx9ZjZEHeKr8yg.png)


## Vertical Scaling

 Upgrading the capacity of a single machine or moving to a new machine with more power is called vertical scaling
.In this we can add more power to your machine by adding better processors, increasing RAM, or other power-increasing adjustments. Vertical scaling can be easily achieved by switching from small to bigger machines but remember that this involves downtime. You can enhance the capability of your server without manipulating your code. 

This is also called the scale-up approach. It is easy to implement, It requires less administrative work and It is used in mid and small-sized companies. 

#### Inter-process communication 
#### Consistent hardware limit

## Horizontal Scaling

In horizontal scaling, we enhance the performance of the server by adding more machines to the network and sharing the processing and memory workload across multiple devices. This approach is the best solution for projects which have requirements for high availability or failover. In this approach, there is no need to change the capacity of the server or replace the server. Also, like vertical scaling, there is no downtime while adding more servers to the network.

This is also called the scale-out approach. It is easy to upgrade, Size, and re-size as required and It can be achieved with the help of a distributed file system, clustering, and load–balancing.

#### Load balancing required
#### Scales well as user increases

### What is load–balancing


 Load balancing is the process of distributing a set of tasks over a set of resources (computing units), to make their overall processing more efficient.
 The efficiency of load-balancing algorithms critically depends on the nature of the tasks. Therefore, the more information about the tasks is available during decision-making, the greater the potential for optimization.

 Load balancing refers to efficiently distributing incoming network traffic across a group of backend servers, also known as a server farm or server pool.

Modern high‑traffic websites must serve hundreds of thousands, if not millions, of concurrent requests from users or clients and return the correct text, images, video, or application data, all in a fast and reliable manner. To cost‑effectively scale to meet these high volumes, modern computing best practice generally requires adding more servers.

The best load balancers can handle session persistence as needed. Another use case for session persistence is when an upstream server stores information requested by a user in its cache to boost performance. Switching servers would cause that information to be fetched for the second time, creating performance inefficiencies.

Hardware and software load balancers may have a variety of special features. The fundamental feature of a load balancer is to be able to distribute incoming requests over a number of backend servers in the cluster according to a scheduling algorithm. Most of the following features are vendor specific:

A load balancer acts as the “traffic cop” sitting in front of your servers and routing client requests across all servers capable of fulfilling those requests in a manner that maximizes speed and capacity utilization and ensures that no one server is overworked, which could degrade performance. If a single server goes down, the load balancer redirects traffic to the remaining online servers. When a new server is added to the server group, the load balancer automatically starts to send requests to it.
Dynamic load balancing algorithms
### Least connection:
 Checks which servers have the fewest connections open at the time and send traffic to those servers. This assumes all connections require roughly equal processing power.
### Weighted least connection:
 It gives administrators the ability to assign different weights to each server, assuming that some servers can handle more connections than others.
### Weighted response time:
 It averages the response time of each server and combines that with the number of connections each server has open to determine where to send traffic. By sending traffic to the servers with the quickest response time, the algorithm ensures faster service for users.
### Resource-based:
 Distributes load based on what resources each server has available at the time. Specialized software (called an "agent") running on each server measures that server's available CPU and memory, and the load balancer queries the agent before distributing traffic to that server.
Static load balancing algorithms
### Round robin:
 Round-robin load balancing distributes traffic to a list of servers in rotation using the Domain Name System (DNS). An authoritative nameserver will have a list of different A records for a domain and provides a different one in response to each DNS query.
Weighted round robin: Allows an administrator to assign different weights to each server. Servers deemed able to handle more traffic will receive slightly more. Weighting can be configured within DNS records.
### IP hash:
 Combines incoming traffic's source and destination IP addresses and uses a mathematical function to convert it into a hash. Based on the hash, the connection is assigned to a specific server.

## Benefits of Load Balancing

#### Reduced downtime
#### Scalable
#### Redundancy
#### Flexibility
#### Efficiency

Load balancing can be useful in applications with redundant communications links. For example, a company may have multiple Internet connections ensuring network access if one of the connections fails. A failover arrangement would mean that one link is designated for normal use, while the second link is used only if the primary link fails.

Using load balancing, both links can be in use all the time. A device or program monitors the availability of all links and selects the path for sending packets. The use of multiple links simultaneously increases the available bandwidth.


## References
https://www.geeksforgeeks.org/

https://www.youtube.com/

https://systemdesignprep.com/scalability
