# ansible-remote-user-creation
## Getting Started

### Prerequisites
```
ansible >= 2.4.0
```

### Installing
```
https://github.com/srekcahrai/remote_user_creation.git
```

## Running
To create only user
```
ansible-playbook main.yml
```

To create only user using ssh passing parameters
```
ansible-playbook -i "127.0.0.1," -e "ansible_port=22 ansible_user=root" main.yml
```

To create user, append ssh key using ssh passing parameters and command parameters
```
ansible-playbook -i "127.0.0.1," -e "ansible_port=22 ansible_user=root username=srekcahrai identity_file=~/devops.pub nopasswd=true sudo=true" main.yml
```
