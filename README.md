<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/79428bc3-0bac-42b8-b79a-10aaca849d21" /># My Cloud Support Lab – AWS EC2 Project

## Project Overview

My Cloud Support Lab is a beginner-level AWS cloud project designed to understand and practise the fundamentals of cloud computing, EC2 instance management, networking, and web server deployment.

In this project, I launched an Amazon EC2 instance, configured the networking and security settings, installed Apache HTTP Server, and hosted a responsive static website using HTML and CSS.

## Project Architecture

![AWS Architecture](architecture.png)

## AWS Services and Technologies Used

- **Amazon EC2:** Hosted the website on a virtual server.
- **Amazon VPC:** Provided the isolated network environment.
- **Internet Gateway:** Enabled internet connectivity.
- **Security Groups:** Controlled inbound traffic to the EC2 instance.
- **Network ACL:** Provided subnet-level network traffic filtering.
- **Route Table:** Defined network traffic routing.
- **Amazon Linux 2023:** Operating system for the EC2 instance.
- **Apache HTTP Server:** Hosted the static website.
- **HTML5 and CSS3:** Used to build the website.

## Project Configuration

| Component | Configuration |
|---|---|
| AWS Region | eu-north-1 |
| Availability Zone | eu-north-1b |
| Instance Type | t3.micro |
| Operating System | Amazon Linux 2023 |
| Web Server | Apache HTTP Server |
| HTTP Port | 80 |
| SSH Port | 22 |
| Web Root Directory | /var/www/html |

## Implementation Steps

### 1. Launch EC2 Instance
- Launched a t3.micro EC2 instance.
- Selected Amazon Linux 2023.
- Configured the required network settings.

### 2. Configure Networking
- Used an existing VPC and public subnet.
- Verified the Internet Gateway.
- Checked the route table and internet route.
- Confirmed public IPv4 address assignment.

### 3. Configure Security Group
Configured inbound rules:

| Type | Port | Source |
|---|---:|---|
| SSH | 22 | My IP address |
| HTTP | 80 | 0.0.0.0/0 |

### 4. Connect to EC2
- Connected using EC2 Instance Connect.
- Accessed the instance through the terminal.

### 5. Install Apache
- Updated the system packages.
- Installed Apache HTTP Server.
- Started and verified the Apache service.

### 6. Deploy Website
- Created HTML and CSS files.
- Stored website files in `/var/www/html`.
- Accessed the website using the EC2 public IPv4 address.
- Tested the website on desktop and mobile screens.

## Project Screenshots

Add your screenshots below. Update the image filenames if yours are different.

### Apache Server Status
![Apache Status](Screenshot%202026-11-07%20222852.png)

### EC2 Instance
![EC2 Instance](Screenshot%202026-11-07%20222556.png)

### Security Group
![Security Group](Screenshot%202026-11-07%20222703.png)

### Website – Desktop View
![Desktop Website](Screenshot%202026-11-07%20222935.png)
![Desktop Website](Screenshot%202026-11-07%20223006.png)
![Desktop Website](Screenshot%202026-11-07%20223016.png)
![Desktop Website](Screenshot%202026-11-07%20223028.png)

### Website – Mobile View
![Mobile Website](Screenshot_20261107-225652_Google)

## Challenges and Troubleshooting

During this project, I practised troubleshooting common cloud deployment issues:

- Understanding EC2 connectivity.
- Configuring SSH and HTTP inbound rules.
- Checking VPC routing and Internet Gateway settings.
- Verifying Apache service status.
- Testing website accessibility.
- Resolving website connection issues.

## Security Practices

- Restricted SSH access to my IP address.
- Allowed HTTP traffic for public website access.
- Used AWS security groups to control instance-level inbound traffic.
- Avoided sharing private keys and sensitive credentials.

## Future Improvements

- Configure HTTPS using SSL/TLS.
- Learn and integrate Amazon S3.
- Implement IAM roles and permissions.
- Configure Amazon CloudWatch monitoring.
- Explore automated deployment.

## What I Learned

Through this project, I gained practical experience with:

- AWS EC2 instance management.
- Basic AWS networking.
- Security group configuration.
- Linux command-line operations.
- Apache web server installation and management.
- Static website deployment.
- Basic cloud troubleshooting.

## Author

**Pankaj Dhavale**

Aspiring Cloud Engineer

This project is part of my hands-on AWS cloud learning journey.
