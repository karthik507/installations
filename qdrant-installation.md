# Qdrant Installation Guide

This guide provides step-by-step instructions to install Qdrant along with the necessary components.

## Official Websites

- **Qdrant**

- [Qdrant Operator GitHub Repository](https://github.com/ganochenkodg/qdrant-operator/tree/main)
- [Qdrant Official Website](https://qdrant.tech/)



## Components

- Qdrant Crds 
- Qdrant Operator

## Steps for Installing Qdrant Operator

### Step 1: Installing Qdrant Operator

1. **Apply the CRDs configuration:**

   ```sh
   kubectl apply -f https://raw.githubusercontent.com/ganochenkodgqdrant-operator/main/deploy/crds/crd-qdrantcluster.yaml

   kubectl apply -f https://raw.githubusercontent.com/ganochenkodg/qdrant-operator/main/deploy/crds/crd-qdrantcollection.yaml
  

2. **Apply the operator configuration:**

    ```sh
    kubectl apply -f operator.yaml



