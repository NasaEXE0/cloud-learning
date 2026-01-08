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
