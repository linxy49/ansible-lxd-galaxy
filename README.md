# ansible-lxd
Ansible Playbook to deploy new LXC containers

## How to use

### Creating containers
```
ansible-playbook -i hosts.target lxc.yml -u <user> \
-e container_name=<container_name> 
-e static_ip=<static_ip> 
-e profile=<profile_required> 
-t create
```

### Delete containers
```
ansible-playbook -i hosts.target lxc.yml -u <user> -e container_name=<container_name> -t delete
```