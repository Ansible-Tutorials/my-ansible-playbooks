## Ansible Playbooks

### Ansible playbooks Verifying playbooks
```bash
ansible-playbook playbook.yml --list-hosts - lista todos os hosts afetados nesse playbook
ansible-playbook playbook.yml --check - executa o playbook em modo de check sem dar apply 
ansible-playbook playbook.yml --list-tasks - lista as tarefas do playbook
ansible-playbook playbook.yml --syntax-check - executa uma verifcacao da sintaxe do YML para do playbook
ansible-playbook --tags=cps playbooks/systems/priority.yml -i inventory.yml
ansible-playbook tags.yml --start-at-task "start NTP service"
```