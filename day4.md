# NAT, routes, Internet Gateway

​
Answer the following questions
​

## 1. What do you think the purpose of an internet gateway is? What would we not be able to do without one?

Connects a local network to the internet. Without one you can't access the internet and cannot be accessed via the internet
​

## 2. Thinking back to a previous session, where do you think you might be using a NAT gateway right now?

Home router

## 3. What IP addresses will be matched by the CIDR block of `0.0.0.0/0`?

All addresses match. It's a wildcard that will be checked last if it doesn't match any other addresses. /0 means it needs to match 0 bits of the address.
​

## 4. In your own words, what is the difference between a NAT gateway and an Internet Gateway? When would you want one over the other?

Internet gateway: doorway between private network and public internet
NAT gateway: connects devices on a private network that want internet access

NATGW used when you want multiple devices on a private network to have internet access and share a single IP address.
IGW when you want unaltered access to the internet on your own unique IP address
