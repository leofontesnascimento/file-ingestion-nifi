# file-ingestion-nifi
This POC (proof of concept) project aims to validate a file ingestion aproach within Apache NiFi.

## Very Important

All data used on this project are fake and had been generated through website:
- https://generatedata.com/

## Pre Configurations

This project considers that you already had Docker and Docker Compose environments pre configured in your Operacional Systems (Preferentially Debian-based Linux Distributions like Ubuntu 20.04 LTS). More details about these configurations should be found on links below:

- https://docs.docker.com/engine/install/ubuntu/
- https://docs.docker.com/engine/install/linux-postinstall/
- https://docs.docker.com/compose/install/

For better experience using Docker, don't forget register on Docker Hub site and do login in your local environment:
- https://hub.docker.com/

## Access Services

### Apache NiFi
1. On your browser access:
```
http://127.0.0.1:8443/nifi/
```

### Apache Hadoop
1. On your browser access namenode service:
```
http://localhost:9870/
```

### Usage

- To execute parquet processors on NiFi it's necessary to use this config as like HDFS Resources path:
```
/opt/hdfs-xmls/core-site.xml,/opt/hdfs-xmls/hdfs-site.xml
``` 
