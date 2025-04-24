📘 What is Ansible?

Ansible is an open-source automation tool used for:

Configuration Management
Application Deployment
Provisioning Infrastructure
Orchestration of IT tasks

It allows you to describe your infrastructure as code, using simple YAML files called playbooks.

⚙️ How Ansible Works

Ansible connects to your systems (called hosts) over SSH and executes tasks remotely. It’s agentless, meaning you don’t need to install anything on the target machines.

🧠 Key Concepts

Playbook: A YAML file that defines what tasks to run on which hosts.
Inventory: A list of target machines (can be static or dynamic).
Task: A single action, like installing a package or restarting a service.
Role: A structured way to organize tasks, variables, templates, and files.
Facts: Automatic system information collected from hosts (e.g. IP, OS).
Module:	A reusable Ansible component to perform tasks (e.g. apt, copy, user).

🚀 Why Use Ansible?

Simple syntax (YAML)
Agentless (no software to install on target machines)
Works on Linux, macOS, cloud, VMs, containers
Scales from one laptop to thousands of servers

🚀 How to Run This Ansible Project

📦 Prerequisites

A GitHub Codespace (Ansible installed with pip install --user ansible)

Basic understanding of YAML

🛠️ Project Structure

ansible-demo/
├── inventory          # Inventory file with target hosts (e.g., localhost)
├── playbook.yml       # Main Ansible playbook
└── vars/
    └── common.yml     # External variables file

▶️ Steps to Run the Playbook

Open Codespace Terminal

Use the built-in terminal in your GitHub Codespace.

Run the playbook

ansible-playbook -i inventory playbook.yml

Expected Output

Prints a greeting message using your system hostname
Creates a file at /tmp/hello_from_var.txt
Shows system facts (RAM, OS, interfaces, etc.)