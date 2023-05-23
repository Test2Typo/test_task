Theoretical Part

I created diagram for application from two part frontend and backend.
Diagram in file architectural_diagram.drawio.png

High Availability and Fault Tolerance:
- Multiple availability zones for distributing resources across data centers
- Load balancing and auto scaling to handle traffic spikes and distribute the load

Disaster Recovery:
- Regular automated backups of databases and storage
- Replication of data and configurations across regions

Auto Scaling:
- Autoscaling groups for dynamically scaling EC2 instances based on traffic or resource usage

Enhanced Security:
- VPC (Virtual Private Cloud) for network isolation
- Security groups and network ACLs for access control

Practical Part 
This repository contains the solution for deploying a Docker application consisting of two components NGINX and PHP. 
The setup utilizes Docker Swarm mode and includes configurations for resource limits and logging of project logs from containers' stdout.

Before getting started, ensure that you have the following prerequisites installed on your machine:
 - Docker: Install Docker
 - Docker Compose: Install Docker Compose

Deployment Steps
Follow the steps below to deploy the Docker application:
1) Clone this repository to your local machine: git clone <repository-url>
2) Navigate to the project directory: cd <project-directory>
3) Deploy the application in Docker Swarm mode: 
 - docker swarm init
 - docker stack deploy -c docker-compose.yml myapp

Cleanup
To remove the deployed application and associated services, run the following command: - docker stack rm myapp
To log out from docker swarm mode: - docker swarm leave --force
