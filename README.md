# oicapm

## OCI APm for weblogic

**TODO for detail steps**
Below is the high level steps

1. Create apm domain. https://docs.oracle.com/en-us/iaas/application-performance-monitoring/doc/get-started-application-performance-monitoring.html
2. Download the agent and install. https://docs.oracle.com/en-us/iaas/application-performance-monitoring/doc/provision-and-deploy-apm-java-agents-linux-application-servers.html
3. Set the classpath of startWeblogic.sh
4. Enable thread snapshot depending on interval default 250ms https://docs.oracle.com/en-us/iaas/application-performance-monitoring/doc/configure-thread-snapshots-apm-agent.html
5. Restart the webologic servers
6. Services/Trace/span will be shown.
7. Jmx metrcis will be under service metrics




## Enable db management vm

**TODO for detail steps**
Below is the high level steps

1. Actually some blog have the details steps https://database-heartbeat.com/2021/09/13/enable-db-mgmt/
2. Refer to offical docs https://docs.oracle.com/en-us/iaas/database-management/doc/get-started-database-management.html
3. In short, Observability & Management->Database Management->Administration->Create an pe 
4. Enable dbsnmp  account with the necessary grant.
5. Put the password in vault, and gramnt polices for database mgt to read from that vault.
6. Enabled db management in Observability & Management->Database Management->Administration
7. Performance hub and awr explorer will be enabled for the databse vm.
6. Service metrics can also be use and build own dashbaord. https://docs.oracle.com/en-us/iaas/Content/Dashboards/home.htm

## Screen shots

WLS Apm example 1
![Apm example](https://github.com/wenjian80/ociapm/blob/main/apm1.JPG)

WLS Apm example 2
![Apm example](https://github.com/wenjian80/ociapm/blob/main/apm2.JPG)

WLS Apm example 3
![Apm Example](https://github.com/wenjian80/ociapm/blob/main/apm3.JPG)

WLS Log analytics 1
![Logan wls example](https://github.com/wenjian80/ociapm/blob/main/loganwls.JPG)

WLS jmx metrix
![OCI Apm wls service metrics](https://github.com/wenjian80/ociapm/blob/main/servicemetrics.JPG)

WLS jmx metrix
![OCI Apm wls service metrics](https://github.com/wenjian80/ociapm/blob/main/apmappmetrics.JPG)


DB Awr explorer
![DB Awr explorer](https://github.com/wenjian80/ociapm/blob/main/arsexplorer.JPG)

DB performance hub
![DB performance hub](https://github.com/wenjian80/ociapm/blob/main/performancehub.JPG)
