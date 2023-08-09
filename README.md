# Infrastructure as Code with Helmfile

This repository contains Infrastructure as Code (IaC) configurations for deploying and managing multiple Kubernetes applications using Helm and Helmfile. The repository is structured to provision the following Helm Charts:

1. **ArgoCD**: A GitOps continuous delivery tool for Kubernetes. It is configured to manage applications using the Apps of Apps pattern.
   
2. **kube-prometheus-stack**: A Helm chart that deploys a full monitoring stack for Kubernetes, including Prometheus, Grafana, and various exporters.
   
3. **ingress-nginx**: A Helm chart for deploying the Ingress Nginx controller, which enables Ingress resource management within Kubernetes.
   
4. **cert-manager**: A Helm chart for deploying Cert Manager, a Kubernetes addon to automate the management and issuance of TLS certificates.

## Apps of Apps Pattern with ArgoCD

The Apps of Apps pattern, also known as "Application Composition" in ArgoCD, is a powerful approach to manage the deployment of complex applications and microservices landscapes. In this repository, the `argocd` directory holds the ArgoCD Application manifests, organized as follows:

- **apps**: This directory contains individual ArgoCD Application manifests for each Helm Chart deployment. Each manifest describes an application using Helmfile as the source of configuration. 

- **helmfile**: The `helmfile` directory contains Helmfile definitions for the Helm Charts mentioned earlier. Each Helmfile is referenced by the respective ArgoCD Application manifests.

By adopting the Apps of Apps pattern, we can easily manage and version our entire Kubernetes application landscape through a single ArgoCD instance.

## Repository Structure

WIP


## Getting Started

1. **Clone this repository:**

WIP

## License
This project is licensed under the MIT License.
