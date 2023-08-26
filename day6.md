# Load Balancing

## Can you decide what type of load balancing from the notes might work best for the following situations;

### A chat service where users maintain active connections for a while

Source request information. Distributing users on their location can help ensure a smooth and uninterrupted experience.
​

### An AI image generation API with paid tiers

Weighted Round Robin. Higher-tier customers get access to servers with larger capacity.

### A social media website that has users all over the world

Least Response Time. Servers with the lowest response times ensures that users experience minimal delays.

### An authorisation service that takes the same amount of time for each request

Least Connection. Distributing requests to servers with the fewest active connections helps evenly spread the load.

### A gaming server that requires low latency

Least Response Time. Low latency is crucial for gaming servers. Prioritising servers with the lowest response times ensures that players experience minimal delays during gameplay.
