# Etcd Package

Etcd is a distributed key-value store designed to securely store data across a cluster. etcd is widely used in production on account of its reliability, fault-tolerance and ease of use.

## Etcd parameters

|Parameter|Description|Type|Default|
|---------|-----------|----|-------|
|pullPolicy|image pull policy|string|IfNotPresent|
|auth.rootPassword|Password for Etcd root user|string|""|

## etcd statefulset parameters

|Parameter|Description|Type|Default|
|---------|-----------|----|-------|
|replicaCount|Number of etcd replicas to deploy|integer|1|
|podManagementPolicy|Pod management policy for the etcd statefulset||Parallel|
|containerPorts.client|Client port to expose at container level|integer|2379|
|containerPorts.peer|Peer port to expose at container level|integer|2380|
|podSecurityContext.fsGroup|Set etcd pod's Security Context fsGroup|integer|1001|
|containerSecurityContext.runAsUser|Set etcd container's Security Context runAsUser|integer|1001|
|||||
|||||
