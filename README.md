# Debian IaC

## Requirements

- Ansible 2.15+ on the control node
- Target hosts running Debian or Ubuntu with `sudo`/root access
- An inventory file listing the target hosts

## Usage

```sh
ansible-playbook -i inventory.ini serv.yaml
```

Optional overrides:

```sh
ansible-playbook -i inventory.ini serv.yaml -e network_interface=ens18
```

```sh
ansible-playbook -i inventory.ini serv.yaml -e skip_on_nat=true
```
