# homework 4 - Ansible 

## Ansible project with 2 roles:
- creating an empty `/etc/iaac` file with `0500` rights
- get the name/version of the Linux distribution

4 machines: 1 master controller - 3 nodes

## Prerequisites:

* Install Ansible on the main server: You will need to have Ansible installed on the main server in order to manage the nodes. You can install Ansible using the package manager for your operating system.

```
sudo apt update -y
sudo apt install python3-pip -y
sudo python3 -m pip install ansible
```

* Configure SSH access: Ansible uses SSH to connect to the nodes. You will need to configure SSH access on the main server and the nodes. 
On the main server, you will need to generate an SSH key ( `ssh-keygen` ) and copy the public key ( ~/.ssh/id_rsa.pub ) to the nodes. 
On the nodes, you will need to add the public key to the authorized_keys file ( ~/.ssh/authorized_keys ).

## Files:

- Creating an inventory file with 4 groups - [hosts](https://github.com/rlnq/homework4/blob/master/hosts)

2 roles: 
- creating a empty file /etc/iaac with rigths 0500 - [empty-file-0500](https://github.com/rlnq/homework4/blob/master/empty-file-0500/tasks/main.yml)
- fetch a linux distro name/version - [distr-name-and-version](https://github.com/rlnq/homework4/blob/master/distr-name-and-version/tasks/main.yml)

Playbook for two roles - [side.yml](https://github.com/rlnq/homework4/blob/master/side.yml)

![image](https://user-images.githubusercontent.com/117667360/209687469-fa2e8623-0752-403d-a426-294038eeef42.png)

