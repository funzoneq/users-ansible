# Ansible Users

A playbook for adding Two P users to linux hosts

## Installation

```
python3 -m venv .venv
source .venv/bin/activate
pip3 install ansible
```

## Running

Edit hosts file to include which servers to run on. Assuming that <user> is the cloud-init user.

Run on a single server:

```
ansible-playbook playbook.yml -u user -b -l 172.16.254.45
```

Run on a group of servers:

```
ansible-playbook playbook.yml -u user -b -l servers
```
