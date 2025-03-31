<h1 align="center">Zabbix Minikube Deploy</h1>

> Zabbix 7.4 version 

## 💻 Installation

###### terminal

```bash
# Initialize Minikube
minikube start

# Apply the YAML files
kubectl apply -f zabbix_db_serviceStateful.yaml
kubectl apply -f zabbix_front_deployment.yaml
kubectl apply -f zabbix_front_service.yaml
kubectl apply -f zabbix_server_deployment.yaml
kubectl apply -f zabbix_server_service.yaml

# Get the Front-End url to log into zabbix
minikube service --all
```

> [!TIP]
> Zabbix default logging credentials are:
> User: Admin
> Password: zabbix