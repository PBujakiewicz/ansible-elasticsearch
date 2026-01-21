# ansible-elasticsearch

## Check inventory
```bash
ansible-inventory --list
```

## Check connection
```bash
ansible all -m ping
ansible elastic_v7_prod -m ping
```

## Test playbook
```bash
ansible-playbook playbooks/main.yaml -e "cluster_group_var=elastic_v7_prod" --syntax-check
ansible-playbook playbooks/main.yaml -e "cluster_group_var=elastic_v7_prod" --check --diff
```

# Run playbooks
```bash
ansible-playbook playbooks/main.yaml -e "cluster_group_var=elastic_v7_prod"
```
