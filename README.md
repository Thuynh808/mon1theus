# Mon1theus

- **Clone repo**

```bash
git clone -b prometheus-nodeexporter-role https://github.com/thuynh808/mon1theus
cd mon1theus
```

- **Configure inventory `hosts`**

```bash
vim inventory
```

- **Install collections**

```bash
./install_req.sh
```

- **Install prometheus**

```bash
ansible-playbook playbooks/prometheus.yaml -vv
```

- **Install snmp_exporter**

```bash
ansible-playbook playbooks/snmp_exporter.yaml -vv
```

- **Install loki**

```bash
ansible-playbook playbooks/loki.yaml -vv
```

- **Install alloy**

```bash
ansible-playbook playbooks/alloy.yaml -vv
```

- **Install grafana**

```bash
ansible-playbook playbooks/grafana.yaml -vv
```
