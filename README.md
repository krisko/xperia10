# xperia ansible

## first install sudo on your phone

```py
pkcon refresh
pkcon install sudo
visudo
# add line: nemo ALL=(ALL) ALL
```

## run ansible playbook

```py
# don't forget to change your phone IP address in inventory/hosts.yml
# then you can run the playbook
ansible-playbook -i inventory/hosts.yml playbooks/xperia.yml
```

# roles description

```
# clock
  - disable clock alarm vibrations
# gps
  - copy gps_on_off script to disable/enable gps (used in situations app)
# camera
  - set advanced-camera as default camera from lockscreen
```
