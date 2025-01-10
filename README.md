# LibreChat Helm Chart

## Description
This Helm chart deploys LibreChat, an open-source chat application, on a Kubernetes cluster.

## Prerequisites
- Kubernetes 1.25+
- Helm 3.0+
- PV provisioner support in the underlying infrastructure
- MongoDB (required for LibreChat)

## Installation

### Add the Helm Repository
```bash
git clone https://github.com/bayzip/librechat-helm.git
cd Charts
helm install librechat ./ -n librechat --create-namespace

# To install with custom values:
helm install librechat ./ -f values.yaml  --create-namespace
```
