# Ansible MERNSTACK Project

This project automates the deployment of a full MERN stack (MongoDB, Express, React, Node) using **Ansible** on virtual machines created with **Multipass**.

---

## 🌐 What is the MERN Stack?

MERN is a JavaScript-based stack used for building modern web applications from end to end:

- **MongoDB** – NoSQL database
- **Express.js** – Backend framework for Node
- **React.js** – Frontend library
- **Node.js** – JavaScript runtime environment

---

## 🔧 Environment Setup Using Multipass

We use **Multipass** to create VMs and **cloud-init** to allow Ansible SSH access to the target machines.

### Machines:

- `webserver`: High-resource VM to run Node, Express, React
- `dbserver`: Runs MongoDB

---

## 📂 Inventory File

We define an Ansible inventory file that includes the `all` ,  `webserver` and `dbserver` hosts grouped accordingly.

---


### Deploy :
# git clone https://github.com/Hossam22elabayati/Ansible_MERNSTACK-.git
# ansible-playbook -i inventory/hosts.ini playbook.yml 
