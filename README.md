[![Build Status](https://drone-ci.hopto.org/api/badges/Diesel-Net/organizr/status.svg)](https://drone-ci.hopto.org/Diesel-Net/organizr)

# organizr
Sets up [Organizr](https://github.com/causefx/Organizr) on my home network. Currently, this is a neat way to provide a quick access and overview to all of the services running on my home lab. It even includes it's own RBAC built-in ;)

## Requirements
- Ansible 2.10+

## Deploy to Docker Swarm
```bash
ansible-playbook deploy.yaml -i inventories/dev/hosts --vault-id ~/.tokens/master_id
```

