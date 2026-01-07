**📦 Jenkins CI/CD Deployment on EC2**

A simple CI/CD pipeline using Jenkins to automatically deploy a project from GitHub to an AWS EC2 instance with Apache.

This project demonstrates hands-on DevOps skills: pipeline setup, GitHub integration, automated build/test/deploy, and EC2 hosting.

🚀 Features**
**
GitHub Integration: Pull code from a GitHub repository.

Jenkins Pipeline: Automated stages: Checkout → Build → Test → Deploy.

EC2 Deployment: Files deployed to /var/www/html on Ubuntu EC2 with Apache.

CI/CD Practice: Demonstrates real-world continuous integration and deployment.

Hands-On Learning: Groovy scripting in Jenkinsfile, pipeline DSL usage.

**🛠️ Tech Stack**
Layer	Tech Used
CI/CD	Jenkins
Source Control	Git / GitHub
Server	AWS EC2 (Ubuntu 22.04)
Web Server	Apache2
Pipeline Script	Jenkinsfile (Groovy DSL)

**📁 Project Structure**
├── Jenkinsfile          # Jenkins pipeline definition
├── index.html           # Sample web page deployed to EC2
└── README.md

**⚡ Pipeline Overview**

The Jenkins pipeline contains the following stages:

Checkout: Pulls latest code from GitHub.

Build: Placeholder for build commands (e.g., Maven, npm, Python).

Test: Placeholder for running automated tests.

Deploy: Copies project files to /var/www/html on EC2.


**🌐 Deployment**

Apache2 is installed on EC2 (/var/www/html)

Ownership is set to Jenkins user to allow non-interactive deployment:  sudo chown -R jenkins:jenkins /var/www/html

After running the Jenkins pipeline, the website is live at your EC2 public IP

**📌 How to Run**

Fork or clone the repository.

Set up an EC2 instance with Ubuntu and Apache installed.

Install Jenkins on EC2.

Add your repository in Jenkins pipeline (Pipeline script from SCM).

Run the pipeline → project files deployed automatically.
