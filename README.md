# Milvus and Attu Installation Guide

This guide provides step-by-step instructions to install Milvus Operator and Attu along with the necessary components.

## Official Websites

- **Milvus**
  - [Milvus Operator Installation Documentation](https://milvus.io/docs/install_cluster-milvusoperator.md)
  - [Milvus Operator GitHub Repository](https://github.com/milvus-io/milvus-operator/tree/main)
- **Attu**
  - [Attu Installation Documentation](https://milvus.io/docs/v2.1.x/attu_install-helm.md)
  - [Attu GitHub Repository](https://github.com/zilliztech/attu)

## Prerequisites

- Cert Manager

## Components

- Milvus Operator
- S3 Bucket with bucket name `milvus`
- Attu for UI
- Kafka Cluster for message stream

## Steps for Installing Milvus Operator and Attu

### Step 1: Installing Milvus Operator

1. **Apply the operator configuration:**

   ```sh
   kubectl apply -f operator.yaml
   kubectl create ns dbaas-registry


### Step 2: Installing

1. **Apply the operator configuration:**

   ```sh
   kubectl create ns attu
   kubectl apply -f attu_deploy.yaml -n attu

2. Change the "host" according to the cluster. And apply the below manifest

   ```sh
   kubectl apply -f attu_ingress.yaml -n attu


