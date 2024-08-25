# Ansible AWS EC2 Automation Project

## Overview

This project demonstrates how to use Ansible to automate various tasks on AWS EC2 instances, including creating instances, setting up passwordless authentication, and conditionally shutting down instances based on their OS type.

## Project Objectives

1. **Automate EC2 Instance Creation**: Using Ansible, create three EC2 instances:
   - Two instances running Ubuntu.
   - One instance running CentOS.

2. **Set Up Passwordless Authentication**: Establish secure, passwordless SSH access between the Ansible control node and the newly created EC2 instances.

3. **Conditional Shutdown**: Use Ansible conditionals to automate the shutdown of only the Ubuntu instances.

## Prerequisites

- Ansible installed on the control node.
- AWS account with proper permissions.
- SSH key pair configured for accessing EC2 instances.
- Ansible inventory and configuration files set up correctly.

## Project Structure

- `playbook_create_instances.yml`: Playbook for creating EC2 instances using Ansible loops.
- `playbook_shutdown_ubuntu.yml`: Playbook for shutting down only the Ubuntu instances using Ansible conditionals.
- `inventory.ini`: Inventory file listing the EC2 instances.
- `ansible.cfg`: Ansible configuration file.
- `scripts/`: Additional scripts if necessary.
