# Blockchain Solution with Hyperledger Fabric + Hyperledger Explorer on Openshift

This is a simple guide to help you implement a complete Blockchain solution using [Hyperledger Fabric v1.3](https://hyperledger-fabric.readthedocs.io/en/release-1.3/whatsnew.html) with [Hyperledger Explorer v0.3.7](https://www.hyperledger.org/projects/explorer) on top of a [Openshift](https://www.openshift.com/) platform.

This solution uses also [CouchDB](http://couchdb.apache.org/) as peer's backend, [Apache Kafka](https://kafka.apache.org/) topics for the orderers and a NFS Server *(Network file system)* to share data between the components.

For more details about hyperledger, please take a look at [original repo](https://github.com/feitnomore/hyperledger-fabric-kubernetes)

This repo use [original repo](https://github.com/feitnomore/hyperledger-fabric-kubernetes) as a baseline for this demo. Many files were added/altered/excluded to support Hyperledger on Openshift.

## PRE-REQ

* oc client
* Ansible

## RUN THIS DEMO

```bash
ansible-playbook install.yml
```

> Remember to update `install.yml` using your openshift credentials. Make sure your user has `cluster-admin` role before running the playbook.