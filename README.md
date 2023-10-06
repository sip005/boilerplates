# boilerplates

### portainer docker
`docker run -d -p 9000:9000 -p 8000:8000 --name=portainer --restart=always -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data portainer/portainer:latest`

`docker run --name owsap --rm -p 3000:3000 --network monitoring-network -v /root/owsap:/var bkimminich/juice-shop`
`docker run -d    --name prometheus02    -p 9090:9090    -v /root/prometheus/prometheus.yml:/etc/prometheus/prometheus.yml    --network monitoring-network    --restart unless-stopped    prom/prometheus    --config.file=/etc/prometheus/prometheus.yml`

`docker run -d \
  --name grafana \
  -p 3001:3000 \
  --net monitoring-network \
  grafana/grafana
`
