### How to run

## Create Ansible vault

 Export `ANSIBLE_VAULT_PASSWORD_FILE` variable 


## Install SSSD and join to Active directory 

```
ansible-playbook join-ad.yml --tags sssd-register
```

## Remove SSSD and leave Acive directory 

```
ansible-playbook leave-ad.yml --tags sssd-unregister -e sssd_remove=True
```
