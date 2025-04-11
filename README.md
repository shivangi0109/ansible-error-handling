# 🛠️ Ansible Playbook: Security Updates & Docker Installation

📘 This Ansible playbook automates essential system updates and Docker setup across your servers.

## ✅ Features

- Installs the latest versions of essential security packages (`openssl`, `openssh`).
- Checks if Docker is already installed on the target system.
- Conditionally installs Docker (`docker.io`) only if it is not already present.
- Ensures the APT package cache is updated before performing installations.
- Uses error handling to allow non-critical tasks to fail without stopping the playbook.

## 🔧 Requirements

- Ansible installed on the control node
- Target hosts defined in your Ansible inventory
- Remote user with `sudo` privileges

## 🚀 Usage

```bash
ansible-playbook -i inventory.ini main.yml
```