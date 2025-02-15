## Don't forget ENV variable
HOST_DOCKER_LOCAL_IP

## Don't forget UFW RULE
Install ufw-docker

sudo ufw allow from <PREMETHEUS_IP_IN_DOCKER(172.16.0.2)> to any port 9100 - for prometheus to have access to node exporter

sudo ufw allow from any to any port 9090 - for web access to prometheus
