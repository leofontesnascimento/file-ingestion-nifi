# file-ingestion-nifi
This project aims to validate a file ingestion aproach within Apache NiFi.

## Access Services

### Apache NiFi
1. On you browser access:
```
http://127.0.0.1:8443/nifi/
```

### Apache Hadoop
1. On you browser access namenode service:
```
http://http://localhost:9870/
```

### Usage

- To execute parquet processors on NiFi it's necessary to use this config as like HDFS Resources path:
```
/opt/hdfs-xmls/core-site.xml,/opt/hdfs-xmls/hdfs-site.xml
``` 