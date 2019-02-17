# run
```bash
# Execute
ansible-playbook -i hosts site.yml

# Specify
ansible-playbook -i hosts site.yml -l raspbian --start-at "Install lsyncd" --step
ansible-playbook -i hosts site.yml -l raspbian --tags "tmp"
ansible-playbook -i hosts site.yml --tags "finalize"

# Dry run
ansible-playbook -i hosts site.yml --check
```
