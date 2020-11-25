# Ping VM
ansible -i hosts.inv -u ricg5 gcp -m ping
# Run Playbook
ansible-playbook playbook.yml 