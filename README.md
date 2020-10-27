# xperia ansible

## install sudo

```py
pkcon refresh
pkcon install sudo
visudo
# add: nemo ALL=(ALL) ALL
```

## run command

```py
# run playbook
ansible-playbook -i inventory/hosts.yml playbooks/xperia.yml
```
