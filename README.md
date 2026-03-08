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
