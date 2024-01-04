# ArgoCD Application Catalog

This repository contains a catalog of sample applications configured to deploy with ArgoCD. 

## Contents

The apps directory contains the following deployed applications:

- **Cert Manager**
- **Cloudflared**
- **Nginx Ingress Controller**
- **Example Ingress Specifications**
- **Linstor CSI** -- contains example specs to deploy linstor storage classes using an existing linstor storage cluster
- **MetalLB**
- **MySQL Operator** -- contains a Kubernetes operator to deploy MySQL DB Instances in the cluster
- **nfs-provisioner** -- contains example specs to deploy storage class that provides persistent volumes from a NFS Share

## Prerequisites

The following tools must be installed:

- Kubernetes 1.16+ 
- ArgoCD -- this can be installed using `argocd-tf-bootstrap` folder. 
- kubectl

## Usage

To deploy an application:

1. Clone this repository
2. Create a new ArgoCD application, pointing to the app directory for the application you want to deploy 
3. Sync the application to deploy to your Kubernetes cluster

For details, please check the documentation inside each application directory.
