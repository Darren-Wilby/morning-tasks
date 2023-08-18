# Designing for failure

​

## Identify the kinds of failure readiness described below, giving your reasoning;

​

### A system that switches to a new server when one fails

Fault Tolerance and High Availability. The system is resilient to failures and can continue functioning with minimal downtime.
​

### Adding replica databases with a master database

Data Redundancy and Disaster Recovery. If the master database fails, the replica databases can take over to ensure data availability and integrity. This approach enhances disaster recovery capabilities by having multiple copies of the data, reducing the risk of data loss in case of failures. ​

### Having a 2-3 colleagues who have access to the master password

Access Management and Contingency Planning. If one person becomes unavailable others can still access and manage the system. It's a form of contingency planning to mitigate risks associated with single points of failure in access control.

### Performing health checks on a server

Monitoring and Proactive Maintenance. This is a proactive approach to failure readiness, as it allows for identifying and addressing potential problems before they escalate and cause downtime or outages.

### Spreading out user requests over multiple machines rather than just one powerful one

Load Balancing and Scalability. Helps ensure that no single server becomes a bottleneck or point of failure due to overwhelming traffic.
