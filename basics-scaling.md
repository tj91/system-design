Scalability
-

In order to use any REST service, the end users need to send requests to the REST server. </p> 
As number of end users grow, the server should be able to handle the incoming requests within the given SLAs, in other words the server should be able to scale.

Scalability can involve :
- **Vertical scaling** is a technique where the server's hardware is replaced by better hardware (i.e. more memory, CPU(or cores) or disk) so that the incoming requests can be served by the single server within the SLAs of the service.
- **Horizontal scaling** requires to add multiple servers so that the requests can be routed to different servers, thereby reducing load on a single machine. 

Comparison between vertical and horizontal scaling

Horizontal scaling 
-
- Requires load balancing
- *Fault tolerant - even if one node goes down, other nodes can serve the request*
- Requires RPCs (slower compared to interprocess)
- Can cause inconsistencies  in case the nodes should have same state
- *Can scale even if number of reqests keep growing.*

Vertical scaling
-
- Doesnt require any load balancing
- Not fault tolerant - we have single point of failure
- *Uses interprocess communication (less network IO compared to horizontal)*
- *No inconsistencies since we have single node to serve request*
- Can scale upto hardware limitations.

Conclusion
-
In system design there are always tradeoffs between different solutions, and based on the **requirements** we design the solution.
