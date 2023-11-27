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
- **Update**

- postgres
- mysql
- docker compose for postgres along with visual tool, prosma
- mongodb versioning conflict
- 

```bash
docker run --name mariadb-container -e MYSQL_ROOT_PASSWORD=1234 -v /root/php/fifty/mariadb_vol:/var/lib/mysql -d mariadb:latest
```

- `docker run` - Command to run a Docker container.
- `--name mariadb-container` - Specifies the name for the container as `mariadb-container`.
- `-e MYSQL_ROOT_PASSWORD=1234` - Sets the root password for the MariaDB instance to `1234`.
- `-v /root/php/fifty/mariadb_vol:/var/lib/mysql` - Mounts the volume located at `/root/php/fifty/mariadb_vol` on the host to `/var/lib/mysql` within the container. This volume will persist MariaDB's data files even if the container is stopped or removed.
- `-d mariadb:latest` - Specifies to run the latest version of the MariaDB Docker image in detached mode (`-d`).
