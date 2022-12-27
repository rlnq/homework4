# homework 4 - Ansible 

4 machines: 1 master controller - 3 nodes

Prerequisites: 

`apt install python3-pip`

`python3 -m pip install ansible`

ssh-keygen on main server → copy .ssh/id_rsa.pud to all hosts in .ssh/authorized_keys

Files:

- Creating an inventory file with 4 groups - [hosts](https://github.com/rlnq/homework4/blob/master/hosts)

2 roles: 
- creating a empty file /etc/iaac with rigths 0500 - [empty-file-0500](https://github.com/rlnq/homework4/blob/master/empty-file-0500/tasks/main.yml)
- fetch a linux distro name/version - [distr-name-and-version](https://github.com/rlnq/homework4/blob/master/distr-name-and-version/tasks/main.yml)

Playbook for two roles - [side.yml](https://github.com/rlnq/homework4/blob/master/side.yml)
