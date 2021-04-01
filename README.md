[![Build Status](https://drone-ci.hopto.org/api/badges/Diesel-Net/organizr/status.svg)](https://drone-ci.hopto.org/Diesel-Net/organizr)

# organizr
Sets up [Organizr](https://github.com/causefx/Organizr) on my internal network. Currently, this is a pretty decent way to provide a quick access and overview to all of the services we are self-hosting. It comes with it's own RBAC so we can delegate to collaborators for convenience.

## Requirements
- Ansible 2.10+

## Installing Dependencies
```bash
ansible-galaxy install -r .ansible/roles/requirements.yaml -p .ansible/roles --force
```

## Deploy to Docker Swarm
```bash
ansible-playbook .ansible/deploy.yaml -i .ansible/inventory/production/hosts --vault-id ~/.tokens/master_id
```

