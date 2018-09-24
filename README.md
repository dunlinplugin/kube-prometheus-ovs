# Traffic monitoring in Kubernetes over the Dunlin Plugin

This Kubernetes deployment installs three compononent for Dunlin Plugin monitoring:

      1. Prometheus server to collect metrics,
      2. OVS-exporter to read information from Open vSwitches using OpenFlow protocol and convert them to Prometheus format,
      3. Grafana dashboard for visualizing the collected metrics.

To use this in your Kubernetes cluster type the following command in your master node:

      $ sudo mkdir /var/lib/prometheus/data; chmod 777 /var/lib/prometheus/data
      $ kubectl apply -f https://dunlin.io/monitoring.yaml
      
      
