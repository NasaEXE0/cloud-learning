# cloud-learning

# Cloud Learning – Week 1 (Linux & EC2)

## Overview
This repository documents my Week 1 cloud learning, focused on Linux fundamentals and deploying a basic web server on AWS EC2.

The goal was to understand how servers work at a low level, including SSH access, package management, networking, and serving web content.

---

## What I did

- Launched a free-tier AWS EC2 instance (Amazon Linux)
- Connected to the server using SSH from Windows PowerShell
- Learned basic Linux navigation and file operations
- Installed software using the system package manager (`yum`)
- Installed and ran the nginx web server
- Configured AWS security groups to allow HTTP traffic on port 80
- Created and served a custom static HTML page

---

## Key concepts learned

- Difference between local machine and remote server
- SSH and port 22
- HTTP vs HTML
- What ports are and how services listen on them
- What a security group is and why ports must be opened
- How nginx serves files in response to HTTP requests

---

## Technologies used

- AWS EC2
- Amazon Linux
- nginx
- SSH
- Linux CLI

---

## Result

The EC2 instance successfully serves a custom HTML page via its public IP address using nginx.

Screenshots below show:
- nginx running as a system service
- the web page being served in a browser

## Screenshots

### nginx running on EC2
![nginx status](screenshots/nginx-status.png)

### Web page served from EC2
![EC2 web page](screenshots/ec2-webpage.png)

## Cloud Learning – Week 2 (Networking Fundamentals)

### Overview
Week 2 focused on understanding how network traffic reaches a server, how web requests are processed, and how to diagnose connectivity issues in a cloud environment.

The emphasis was on learning how to verify each layer of the network stack (DNS, IP addressing, ports, and services) and how to troubleshoot common access problems.

---

### What I did
- Learned the difference between IP addresses and domain names
- Understood how DNS resolves a domain name to an IP address
- Studied the HTTP request lifecycle from browser to server and back
- Learned the purpose of common ports (22, 80, 443)
- Used `curl` to test HTTP endpoints from the command line
- Verified connectivity using both domain names and raw IP addresses
- Modified EC2 security group rules to allow and block traffic
- Intentionally broke HTTP access by removing port 80 and restored it
- Diagnosed issues by testing locally on the server versus externally

---

### Key concepts learned
- DNS resolution (browser → resolver → authoritative DNS)
- Endpoints as a combination of IP/domain, port, and service
- Difference between application-level issues and network-level issues
- How security groups control inbound traffic to EC2 instances
- How to isolate failures using `curl`, `nslookup`, and SSH
- Why a service can work locally but be unreachable from the internet

---

### Technologies & tools used
- AWS EC2
- Amazon Linux
- nginx
- SSH
- `curl`
- PowerShell
- Linux networking tools

---

### Result
The EC2 instance is reachable via HTTP from the public internet.

I am able to verify DNS resolution, test endpoints using `curl`, and diagnose connectivity issues by identifying whether failures occur at the application, operating system, or AWS networking layer.
