corri isto
instalar agentes

```
echo "" > agents_to_install.csv && \
> echo '"projects/ascn2223g9/zones/us-central1-a/instances/gke-ascn-cluster-ascn-pool-01252091-16kp","[{""type"":""ops-agent""}]"' >> agents_to_install.csv && \
> echo '"projects/ascn2223g9/zones/us-central1-a/instances/gke-ascn-cluster-ascn-pool-01252091-4z5g","[{""type"":""ops-agent""}]"' >> agents_to_install.csv && \
> curl -sSO https://dl.google.com/cloudagents/mass-provision-google-cloud-ops-agents.py && \
> python3 mass-provision-google-cloud-ops-agents.py --file agents_to_install.csv
```


```bash
gcloud cloud-shell ssh --command="echo "" > agents_to_install.csv && echo '\"projects/ascn2223g9/zones/us-central1-a/instances/gke-ascn-cluster-ascn-pool-01252091-16kp\",\"[{\"\"type\"\":\"\"ops-agent\"\"}]\"' >> agents_to_install.csv && curl -sSO https://dl.google.com/cloudagents/mass-provision-google-cloud-ops-agents.py && python3 mass-provision-google-cloud-ops-agents.py --file agents_to_install.csv"
```

```bash
echo '\"projects/ascn2223g9/zones/us-central1-a/instances/gke-ascn-cluster-ascn-pool-01252091-16kp\",\"[{\"\"type\"\":\"\"ops-agent\"\"}]\"' >> agents_to_install.csv
```