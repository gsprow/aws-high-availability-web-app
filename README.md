# Highly Available AWS Web Application

## Overview

This project demonstrates the deployment of a highly available web application using Amazon Web Services. The environment distributes traffic across multiple EC2 instances located in separate Availability Zones through an Application Load Balancer.

The infrastructure was designed to demonstrate fault tolerance, load balancing, and scalable cloud architecture commonly used in production AWS environments.

---

## Business Scenario

A growing company requires a public-facing web application that remains available even if a server fails.

To accomplish this, traffic is distributed across multiple EC2 web servers using an Application Load Balancer while leveraging Target Groups and Auto Scaling capabilities to maintain application availability.

---

## AWS Services Used

- Amazon EC2
- Amazon VPC
- Public Subnets
- Security Groups
- Application Load Balancer
- Target Groups
- Launch Templates
- Auto Scaling Groups
- Amazon Linux 2023

---


## Deployment Steps

1. Created a custom Amazon VPC.
2. Configured two public subnets across separate Availability Zones.
3. Built an Application Load Balancer.
4. Configured a Target Group with HTTP health checks.
5. Created a Launch Template.
6. Deployed EC2 web servers.
7. Registered EC2 instances with the Target Group.
8. Verified healthy targets.
9. Tested application availability through the Load Balancer.

---

## High Availability Demonstration

The application remained accessible through the Application Load Balancer while requests were distributed across multiple EC2 instances.

This architecture provides a foundation for fault-tolerant web applications capable of supporting future Auto Scaling and production workloads.

---

## Screenshots

See the **screenshots** folder.

---

## Lessons Learned

- Application Load Balancer configuration
- Target Groups
- Health Checks
- Multi-AZ architecture
- EC2 Launch Templates
- Security Groups
- High Availability design
- Load balancing concepts

---

## Future Improvements

- HTTPS using ACM
- Route53 custom domain
- Auto Scaling policies
- CloudWatch alarms
- Terraform deployment
- CI/CD using GitHub Actions
