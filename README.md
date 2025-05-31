# 🚀 Flask Docker Deployment with Ansible + Nginx + UFW

This project automates the deployment of a simple Flask web application inside a Docker container, sets up an Nginx reverse proxy, and configures the firewall using Ansible.

## 📦 What it Does

- Installs Docker and Docker Compose
- Builds and runs a Flask app inside a container
- Installs and configures Nginx as a reverse proxy to Flask
- Enables UFW and opens ports 22, 80, 443
- Structured with Ansible roles and templates

## 🧰 Technologies Used

- Ansible
- Docker + Compose
- Flask (Python 3)
- Nginx
- UFW (Uncomplicated Firewall)

## 🗂️ Project Structure

flask-docker-deploy/
├── inventory
├── deploy.yml
├── .gitignore
├── README.md
├── roles/
│ ├── docker/
│ ├── flask_app/
│ ├── nginx/
│ └── firewall/


## 🛠️ How to Use

1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/flask-docker-deploy.git
   cd flask-docker-deploy

Run the playbook:

ansible-playbook -i inventory deploy.yml --ask-become-pass

⚠️ Prerequisites
Ubuntu-based system

Python 3 and Ansible installed

Sudo access