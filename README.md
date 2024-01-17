First install k3s using the following command:

```curl -sfL https://get.k3s.io | INSTALL_K3S_EXEC="--disable=metrics-server" sh -```

Then create the namespace monitoring.

Then you can apply the folders/files in the following order:  
1. metrics-server-components.yaml  
2. kubernetes-persistent-volume/  
3. kubernetes-prometheus/  
4. kube-state-metrics-configs/  
5. kubernetes-node-exporter/  
6. kubernetes-grafana/

Finally import the grafana-dashboard.json in the Grafana application.  
