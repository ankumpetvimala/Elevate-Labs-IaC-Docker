
# DevOps Internship Task 3: Infrastructure as Code with Terraform

This repository contains the solution for provisioning a Docker container (Nginx) using **Terraform** on an AWS **t2.micro** Ubuntu instance.

---

## Task Overview

Provision a local **Docker container** using **Terraform** on a provisioned AWS EC2 instance.

---

## Tools Used

- Terraform
- Docker
- AWS EC2 (Ubuntu)
- Bash/CLI

---

## Deliverables

   main.tf
   
   execution logs.

##  Steps Performed

1. Launched a t2.micro EC2 Ubuntu instance on AWS.
2. Installed Docker and Terraform on the instance.
3. Wrote a `main.tf` file to define Docker provider and Nginx container.
4. Ran Terraform commands:
   ```bash
   terraform init       # initialize the project
   terraform plan       # review the execution plan
   terraform apply      # provision the infrastructure
   terraform state list # list managed resources
   terraform destroy    # destroy provisioned resources

## Files 

- main.tf: Terraform configuration file.

- init.log: Terraform initialization log.

- plan.log: Terraform plan log.

- apply.log: Terraform apply log.

- state.log: Terraform state list log.

- destroy.log: Terraform destroy log.


 ## Outcome
 
 Successfully provisioned and destroyed an Nginx container using Terraform, demonstrating Infrastructure as Code (IaC) principles.

 ## Interview Q&A
 
### 1 What is Infrastructure as Code (IaC)?

IaC is the process of managing infrastructure using configuration files rather than manual provisioning, enabling version control, repeatability, and automation.

### 2 How does Terraform work?

Terraform uses declarative configuration files to describe infrastructure. It compares the desired state with the current state and applies necessary changes through API calls.

### 3 What is a Terraform state file?

The terraform.tfstate file tracks the real-world resources Terraform manages, mapping them to the configuration defined in your .tf files.

### 4 Difference between terraform plan and terraform apply?

plan: Previews changes without applying them.

apply: Applies the changes to match the defined configuration.

### 5 What are Terraform providers?

Providers are plugins that interact with APIs (e.g., AWS, Docker, Azure). They define the available resources and handle provisioning tasks.

### 6 What is resource dependency in Terraform?

When one resource depends on another. Terraform auto-detects dependencies, but depends_on can be used to define explicit relationships.

### 7 How do you handle secret variables?

Use variable "secret" { sensitive = true }

Environment variables

External tools like HashiCorp Vault

Never commit secrets to GitHub

### 8 Explain the benefits of Terraform

Version-controlled infrastructure

Consistent environments

Documentation of infrastructure

Automation reduces human error

Multi-cloud support

Reusable modules

Change preview with plan


