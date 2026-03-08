# devops-multi-server-automation
This project demonstrates a real-world DevOps automation workflow using Terraform, AWS, SSH, and Jenkins.
```
                   +---------------------+
                   |     GitHub Repo     |
                   |  DevOps-Automation  |
                   +----------+----------+
                              |
                              |
                       Infrastructure as Code
                         (Terraform)
                              |
                              v
                     +------------------+
                     |   AWS EC2 Server |
                     | Ubuntu Instance  |
                     +------------------+
                              ^
                              |
                        SSH Authentication
                              |
                   +----------+----------+
                   |     Home Server     |
                   |  (SSH Key Creator)  |
                   +----------+----------+
                              |
                              |
                        Jenkins Pipeline
                              |
                +-------------+-------------+
                |                           |
                v                           v
        +---------------+           +---------------+
        | AWS EC2 Node  |           | Raspberry Pi  |
        | 54.**.**.**   |           | 192.168.**.** |
        +---------------+           +---------------+
                |                           |
                +-----------+---------------+
                            |
                            v
                    Automation Tasks
                    -----------------
                    • SSH Test
                    • Reboot Servers
                    • Update Packages
                    • Upgrade Packages
```

```
devops-multi-server-automation
│
├── terraform
│   ├── main.tf
│   ├── variables.tf
│   ├── outputs.tf
│   └── provider.tf
│
├── jenkins
│   └── Jenkinsfile
│
├── diagrams
│   └── architecture.png
│
├── scripts
│   └── ssh-test.sh
│
├── docs
│   └── setup-guide.md
│
└── README.md
```
## Technologies Used

- Terraform
- Jenkins
- AWS EC2
- Raspberry Pi
- SSH
- GitHub

## Features

- Infrastructure provisioning with Terraform
- SSH key-based authentication
- Jenkins pipeline automation
- Multi-server management
- Automated updates and upgrades
- Remote reboot automation

## Architecture

Home Server → Terraform → AWS EC2  
Home Server → Jenkins → SSH → Multiple Servers

## Automation Tasks

- SSH connectivity testing
- Package updates
- System upgrades
- Server reboot

## Jenkins Pipeline

Automates maintenance tasks across multiple nodes simultaneously.

## Skills This Project Demonstrates

This repo shows strong knowledge of:

Terraform

Jenkins

GitHub

Amazon EC2

Infrastructure as Code

CI/CD pipelines

SSH automation

Multi-node management

# Diagram 
<img width="1021" height="837" alt="image" src="https://github.com/user-attachments/assets/39f15188-dd87-4e16-a6a7-fc07efd0de7d" />
<img width="853" height="847" alt="image" src="https://github.com/user-attachments/assets/0ab009b8-a736-432d-a74f-98c47c8d1bb8" />
<img width="1887" height="648" alt="image" src="https://github.com/user-attachments/assets/6b4eac6b-3f73-4f73-8eca-7d1b7fb16f68" />


