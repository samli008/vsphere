## vsphere-vCenter-deploy
Ansible playbook to automate deployment of vCenter, nested ESXi hosts
![](./img/vsan.jpg)
## Table of Contents

This repository will be used to hold an Ansible Playbook to deploy and configure vCenter and nested ESXi VMs 

## Setup

master branch is updated for vSphere 6.7.
for olther versions see pre-67 branch!

### Dependencies
```
yum -y  install sshpass python-pip git 
pip install vim
pip install pyvmomi
```
Place the ESXi and VCSA ISOs in /root/

### Edit answersfile.yml

Edit answersfile.yml according to your infrastructure!

## Usage
```
ansible-playbook deploy.yml
```
## Limitations
Ansible => 2.7 is required
ESXi version 6.7 and above is supported
VCSA version 6.7 and above is supported
```
yum -y remove ansible
pip install ansible==2.7 -i https://mirrors.aliyun.com/pypi/simple
```
## Development
TODO: External PSC for vSphere 6.7
VMware internal
