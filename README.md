# Static Website Deployment on AWS EC2 using Nginx

## Project Overview

This project demonstrates the deployment of a static website on an AWS EC2 instance using Nginx as the web server. Git was used as part of the deployment workflow to manage and transfer the website source code to the server.

The project helped me gain practical experience with cloud infrastructure, Linux server administration, web server configuration, and basic deployment troubleshooting.

## Project Objectives

- Launch and access an AWS EC2 instance.
- Connect to the server using SSH.
- Use Git to manage and deploy website files.
- Configure Nginx to serve a static website.
- Verify the website through a web browser.
- Practice Linux commands and troubleshoot deployment issues.

## Technologies Used

- **Cloud Platform:** Amazon Web Services (AWS)
- **Compute Service:** Amazon EC2
- **Operating System:** Amazon Linux (exact version to be confirmed)
- **Web Server:** Nginx
- **Version Control:** Git
- **Frontend:** HTML, CSS
- **Remote Access:** SSH

## Architecture

```text
          User / Web Browser
                  |
                  | HTTP request
                  v
          EC2 Public IP
                  |
                  v
          AWS Security Group
                  |
                  v
           EC2 Instance
           (Amazon Linux)
                  |
                  v
              Nginx
                  |
                  v
        Static Website Files
           (HTML and CSS)
```

Git is used to manage and deploy the website source code to the EC2 instance.

## Deployment Workflow

### 1. Launch an EC2 Instance

Created an AWS EC2 instance to host the static website.

### 2. Connect to the Instance

Used SSH and key-pair authentication to access the Linux server.

### 3. Install and Configure Nginx

Set up Nginx as the web server to serve the static website.

### 4. Deploy Website Files Using Git

Used Git as part of the deployment workflow to obtain the website source code on the server.

**Note:** The exact Git commands and repository URL used during deployment can be added after verification.

### 5. Configure Network Access

Reviewed EC2 security group settings to allow the required web traffic.

For a public website, HTTP traffic typically uses TCP port 80. SSH access should be restricted to the administrator's trusted IP address wherever practical.

### 6. Verify the Deployment

Opened the EC2 public IP address in a web browser and verified that the website was accessible.

## Repository Contents

- `index.html` — HTML file containing the website structure.
- `style.css` — CSS file containing the website styling.

## Skills Practiced

- AWS EC2 instance management
- Linux command-line operations
- SSH connectivity and key-pair authentication
- Git-based source code deployment
- Nginx web server fundamentals
- Basic cloud networking and security group configuration
- Website testing and troubleshooting

## Challenges and Troubleshooting

This project provided practical exposure to server setup, connectivity, and deployment troubleshooting.

Specific errors, their root causes, and their resolutions will be documented here after verifying the issues encountered during the project.

## Future Improvements

- Automate deployment using a CI/CD pipeline.
- Integrate GitHub with an automated deployment workflow.
- Add screenshots of the running website and AWS configuration.
- Improve server monitoring and logging.
- Explore containerizing the application using Docker.

## Project Status

**Completed and tested.**

The static website was deployed on AWS EC2 using Nginx and verified through a web browser.

## Author

**Kapa Ravi Kumar**

Aspiring DevOps Engineer

- GitHub Profile: https://github.com/kaparavikumar7-tech
- Project Repository: https://github.com/kaparavikumar7-tech/devops-static-website
- Email: ravikumarkapa7@gmail.com

## Troubleshooting and Lessons Learned

During this AWS EC2 static website deployment project, I encountered issues involving Nginx command availability and SSH connectivity.

### Issue 1: `bash: nginx: command not found`

**Symptom**

The Linux shell returned the error:

```text
bash: nginx: command not found
```

**Investigation**

- Identified that the shell could not locate the Nginx command.
- The next diagnostic step is to verify whether Nginx is installed and whether its executable is available in the system's PATH.

**Possible Root Cause**

Nginx may not have been installed, or its executable may not have been accessible through the current PATH. The exact cause requires verification.

**Resolution**

The website was eventually deployed and tested successfully using Nginx. However, the exact corrective command used to resolve this error has not yet been confirmed.

**Key Learning**

When a command is not found, verify software installation and command availability before attempting further configuration.

### Issue 2: SSH Connectivity to AWS EC2

**Symptom**

An SSH connection issue occurred while accessing the EC2 instance.

**Investigation**

SSH connectivity requires checking the connection details, instance status, authentication key, network reachability, and applicable security group rules.

**Root Cause**

The exact cause of the original SSH issue has not yet been confirmed.

**Resolution**

SSH access was eventually established for the project. The exact corrective action used to resolve the original connection issue still needs to be documented.

**Key Learning**

Troubleshoot SSH failures systematically by checking the error message, instance status, connection details, authentication, and network access.

### Troubleshooting Summary

| Issue | Status |
|---|---|
| Nginx command not found | Encountered; exact fix needs verification |
| SSH connectivity | Encountered; exact cause and fix need verification |
| Website deployment | Completed and tested |

