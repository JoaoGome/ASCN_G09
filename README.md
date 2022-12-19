# ASCN_G09

[nota] antes de poder correr os comandos e preciso ter a chave do gke em ~/keys/key.json

criar o cluster:
ansible-playbook create-gke-cluster.yml -i inventory/gcp.yml

destruir o cluster:
ansible-playbook destroy-gke-cluster.yml -i inventory/gcp.yml
