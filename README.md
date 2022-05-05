# Etcd Package

Etcd is a distributed key-value store designed to securely store data across a cluster. etcd is widely used in production on account of its reliability, fault-tolerance and ease of use.

## Etcd parameters

|Parameter|Description|Type|Default|
|---------|-----------|----|-------|
|pullPolicy|image pull policy|string|IfNotPresent|
|auth.rootPassword|Password for Etcd root user|string|""|
