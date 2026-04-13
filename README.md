# Ansible Nginx Deployment Project

## Overview
This project demonstrates how to use Ansible to automate the configuration of a Linux server in AWS.

The playbook installs nginx, ensures the service is running and enabled, and deploys a custom web page using Ansible templates.

## Technologies Used
- Ansible
- AWS EC2 (Amazon Linux)
- Nginx
- YAML (Ansible Playbooks)
- Jinja2 (Templates)

## Project Structure
ansible-nginx-project/
	inventory/
		inventory.ini
	playbooks/
		install_nginx.yml
	templates/
		index.html.j2
	README.md


## What the Playbook Does
- Installs nginx using the dnf package manager
- Ensures nginx is started and enabled on boot
- Deploys a dynamic index.html page using a Jinja2 template
- Uses variables to customize the deployed content

## How to Run
1. Clone or copy the project to your system
2. Update the inventory file if needed
3. Run the playbook:

```bash
ansible-playbook -i inventory/inventory.ini playbooks/install_nginx.yml
