# Ansible and Docker-compose

An ansible playbook with examples on how to install: 
- a simple packages like zip and vim
- a simple create a folder and copy/create a file in it 
- Docker Engine, Python3 and Docker-compose from the repository

using simple module apt,file and copy
each from a another role


## Prerequesits:

* Installed Ansible


## How to setup:

start with clone this repository
```bash
git clone https://github.com/isaacTadela/Ansible.git
cd Ansible/
```

and run 
```bash
sudo ansible-playbook playbook.yaml --connection=local
```


## Notes:

- Creates and tested on an Ubuntu 18.04 VM with 2 CPU's and 2048 MB Ram memory

- In case you want to apply it on real machines you will need to 
  update the inventory because it currently contains only the localhost
  (Inventory = all the ip address of the machines involved in task executions)
```bash
[servers]
localhost
```
