# Ansible and Docker-compose

An ansible playbook with examples on how to: 
- Install a simple packages like zip and vim
- Create a folder and copy/create a file in it 
- Install Docker Engine, Python3 and Docker-compose from the repository

 using the simple modules apt,file and copy
 and each in a another role


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

Creates and tested on an Ubuntu 18.04 VM with 2 CPU's and 2048 MB Ram memory

In case you want to apply it on real machines you will need to:
  - update the inventory (host file) because it currently contains only the localhost
  - remove the 'connection' flag
  - take care of the shh key
  
  (Inventory = all the ip address of the machines involved in task executions)
```bash
[servers]
localhost
```
