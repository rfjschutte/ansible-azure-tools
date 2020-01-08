# ansible-azure-tools

Tools to create, deallocate, remove and show hosts running in Azure

## Command examples

***Show hosts in Azure cloud***

```bash
ansible-playbook -i ./azure_rm.py show_hosts.yml
```
***Create new host***

```bash
ansible-playbook -i ./azure_rm.py create_host.yml -e "resource_group=rg_ansible_test vm_name=test123"
```

***Shutdown host***

```bash
ansible-playbook -i ./azure_rm.py shutdown_host.yml -e "resource_group=rg_ansible_test vm_name=test123"
```

***Remove a host***

```bash
ansible-playbook -i ./azure_rm.py remove_host.yml -e "resource_group=rg_ansible_test vm_name=test123"
```
