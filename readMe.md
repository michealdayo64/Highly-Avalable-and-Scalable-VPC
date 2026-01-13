# Creating a Scalable and Highly Available Private Netweok Environment
Creating a Scalable and Highly Available Private Network Environment using Amazon Elastic Load Balancer (ELB) and Amazon EC2 Auto Scaling on Amazon Web Services (AWS).

## Objective of this Lab
1. Project Architecture
2. Inspect a virtual private cloud (VPC).
3. Update a network to work across multiple Availability Zones.
4. Create an Application Load Balancer.
5. Create a launch template.
6. Create an Auto Scaling group.
7. Set an alarm on a system metric to initiate auto scaling.
8. Test load balancing and automatic scaling.



## 1. Project Architecture
<img width="654" height="350" alt="Screenshot 2026-01-09 at 18 58 44" src="https://github.com/user-attachments/assets/c8c23047-0e7c-4193-bb9d-e57845b2379a" />

## Inspect a virtual private cloud (VPC).
By default, i have two available zones, with two public subnet and four private subnet. i have a nat-gateway in public subnet one, a cafe application server running inside an EC2 instance placed inside private subnet 1, and RDS primary database inside private subnet 3. But the problem with architecture is that it's not highly avaiable and scalalble.

## Update a network to work across multiple Availability Zones.
I will be creating another nat-gateway inside public subnet 2. A NAT gateway allows instances that do not have a public IP address to access the internet.
<img width="1440" height="759" alt="Screenshot 2026-01-13 at 17 41 33" src="https://github.com/user-attachments/assets/80dd939d-2a3b-4854-93b4-e5f25fa701bd" />


## Create an Application Load Balancer.


## Create a launch template.
<img width="1438" height="755" alt="Screenshot 2026-01-13 at 17 43 16" src="https://github.com/user-attachments/assets/08bbe875-1947-4578-a47d-b713f211650e" />


## Create an Auto Scaling group.
<img width="1440" height="757" alt="Screenshot 2026-01-13 at 17 44 12" src="https://github.com/user-attachments/assets/09623c84-45fa-42c3-af28-906e4d2f5a3d" />


## Set an alarm on a system metric to initiate auto scaling.

## Test load balancing and automatic scaling.
