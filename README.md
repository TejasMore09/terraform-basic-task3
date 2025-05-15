# terraform-basic-task3
# Terraform Docker Task

This repository contains the Terraform configuration files to automate the deployment of an Nginx Docker container.

## Project Overview

The task involves using Terraform to:

- Set up the Docker provider
- Define a Docker image resource for Nginx
- Create and run a Docker container based on the Nginx image
- Map the container port "80" to the host port "8090" for external access

By applying this configuration, Terraform automates the process of running an Nginx web server inside a Docker container on your local machine.

## Files Included

- "main.tf": The main Terraform configuration file defining provider, Docker image, and container resources.
  ".terraform.lock.hcl" and ".terraform/": Terraform dependency and plugin files (auto-generated).
- "terraform.tfstate" and "terraform.tfstate.backup": Terraform state files (auto-generated).

## Notes

- The container port "80" is mapped to host port "8090". Make sure port "8090" is free before applying.
- If the port is already in use, Terraform will fail to start the container.
- To destroy the infrastructure, run "terraform destroy".
