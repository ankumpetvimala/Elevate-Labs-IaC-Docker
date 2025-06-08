DevOps Internship Task 3: Infrastructure as Code with Terraform
This repository contains the solution for provisioning a Docker container using Terraform on an AWS t2.micro Ubuntu instance.

Task Overview
Objective: Provision a local Docker container using Terraform.
Tools: Terraform, Docker.
Deliverables: main.tf, execution logs.
Steps Performed
Set up an Ubuntu t2.micro instance with Docker and Terraform.
Wrote main.tf to provision an Nginx container.
Executed:
terraform init (see init.log)
terraform plan (see plan.log)
terraform apply (see apply.log)
terraform state list (see state.log)
terraform destroy (see destroy.log)
Verified the container with docker ps and curl localhost:8080.
Files
main.tf: Terraform configuration file.
init.log: Terraform initialization log.
plan.log: Terraform plan log.
apply.log: Terraform apply log.
state.log: Terraform state list log.
destroy.log: Terraform destroy log.
Outcome
Successfully provisioned and destroyed an Nginx container using Infrastructure as Code principles with Terraform.

Interview Questions Answers
What is IaC? Infrastructure as Code is managing and provisioning infrastructure through machine-readable definition files rather than manual processes.

How does Terraform work? Terraform uses declarative configuration files to define desired infrastructure state, then makes API calls to cloud providers to create/modify resources to match that state.

What is Terraform state file? The state file (terraform.tfstate) tracks the relationship between real-world resources and your configuration, storing metadata about managed infrastructure.

Difference between apply and plan plan shows what changes Terraform will make without actually making them. apply executes the changes after showing the plan.

What are Terraform providers? Plugins that interact with APIs of cloud providers and other services. They define resource types and handle API calls (e.g., Docker, AWS, Azure providers).

What is resource dependency? When one resource relies on another. Terraform automatically handles most dependencies, but you can explicitly define them with depends_on.

How do you handle secret variables? Use Terraform variables with sensitive=true, environment variables, or secret management tools like HashiCorp Vault. Never commit secrets to version control.

Explain the benefits of Terraform

Version-controlled infrastructure
Consistent environments
Documentation of infrastructure
Automation reduces human error
Multi-cloud support
Reusable modules
Change preview with plan
About
Task-3

Resources
 Readme
 Activity
Stars
 0 stars
Watchers
 1 watching
Forks
 0 forks
Report repository
Releases
No releases published
Packages
No packages published
Languages
HCL
100.0%
Footer
© 2025 GitHub, Inc.
Footer navigation
Terms
Privacy
Security
Status
Docs
Contact
Manage cookies
Do not share my personal information
Pravalika-27/Elevate-Labs-IaC-Docker: Task-3
 
