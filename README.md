# CORD Bachelor Degree Thesis

Additional files for SiaB integration with BMv2 P4 switch and NG-SDN interfaces:

### Network Configuration File

Configuration file ([*netcfg.json*](https://github.com/marcllena/SiaB-P4/blob/main/netcfg.json)) to upload to ONOS in order to discover the deployed BMv2 switch. The file contains the corresponding switch management address, drivers, pipeline configuration... and can be posted to ONOS with the following command: 

```
curl --user onos:rocks -X POST -H "Content-Type: application/json" \
http://127.0.0.1:30120/onos/v1/network/configuration/ -d @./netcfg.json
```


### Grafana SiaB Dashboard:

Dashboard made up by Docker Monitoring and Node Exporter dashboards.

To import it from the Grafana GUI, we must select the option “Import dashboard” at the right of the dashboard list. We can then paste the [Dashboard JSON](https://github.com/marcllena/grafana-SiaB-dashboard/blob/main/SiaB_Monitoring_Dashboard.json). 

Marc Llena
