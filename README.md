# docker-compose-influxdb-telegraf-grafana
This is a docker compose to create containers about InfluxDB, Telegraf and Grafana.

### Infrastructure model
edit: 
	#influxDB:
	- INFLUXDB_DB=influx
	- INFLUXDB_ADMIN_USER=admin
	- INFLUXDB_ADMIN_PASSWORD=admin
	#Grafana:
	- GF_SECURITY_ADMIN_USER=admin
	- GF_SECURITY_ADMIN_PASSWORD=admin
	- GF_INSTALL_PLUGINS=flant-statusmap-panel,grafana-clock-panel
Apply:

```bash
docker-compose up -d
```
