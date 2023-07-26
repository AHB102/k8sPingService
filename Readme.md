Ping service

This is a small program that repeatedly pings a list of URLs. It was designed to run inside a Kubernetes cluster to monitor a list of internal service endpoints during network upgrades.

Usage

To use the ping service, you can apply the ping-service.yaml file directly. This will cause the service to ping https://google.com as an example. To customize the service, download the file and update the PING_URLS environment variable.

To apply the ping service:

kubectl apply -f ./ping-service.yaml
To view the logs of the ping service:

kubectl logs -f [name]