<h1 align="center">Zabbix Minikube Deploy</h1>

> Zabbix 7.4 version 

## 💻 Installation

###### terminal

```bash
# Initialize Minikube
minikube start

# Apply the YAML files
kubectl apply -f .

# Get the Front-End url to log into zabbix
minikube service --all
```

> [!TIP]
> Zabbix default logging credentials are:
> User: Admin
> Password: zabbix
