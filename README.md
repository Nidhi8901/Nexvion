# Nexvion DevOps & Cloud-Native Delivery Platform

Nexvion is a ready-made static e-commerce application provided for the Davine Technologies DevOps project. This repository contains the DevOps and cloud-native implementation built around the application.

## Technology Stack

- Git and GitHub
- Linux and Bash
- Docker
- Docker Compose
- Jenkins CI/CD
- Trivy Security Scanning
- Terraform
- Ansible
- AWS EC2
- Kubernetes / Kind
- Helm
- Prometheus
- Grafana
- Elasticsearch
- Logstash
- Kibana
- AI-Assisted Incident Analysis

## CI/CD Flow

GitHub -> Jenkins -> Validation -> Security Scan -> Docker Build -> Image Scan -> Docker Registry -> Deployment -> Verification

## Infrastructure

Terraform provisions the AWS networking and EC2 infrastructure.

Ansible configures the EC2 instance and deploys the Nexvion Docker container.

## Kubernetes

The Kubernetes implementation includes:

- Namespace
- Deployment
- Pods
- Service
- ConfigMap
- Secret
- Ingress
- Scaling
- Rolling updates
- Helm packaging

## Monitoring

Prometheus collects Kubernetes metrics and Grafana provides operational dashboards for Nexvion.

## Centralized Logging

Logstash collects Nexvion container logs, Elasticsearch stores and indexes them, and Kibana provides centralized log investigation using the Nexvion Logs data view.

## Security

- Trivy filesystem and secret scanning
- Docker image vulnerability scanning
- Runtime Kubernetes secrets
- Privilege escalation disabled
- Restricted Linux capabilities
- RuntimeDefault seccomp profile
- AWS SSH access restrictions
- IMDSv2
- Encrypted EC2 root storage

## AI-Assisted DevOps

AI assists with:

- Error classification
- Incident severity assessment
- Possible root-cause identification
- Investigation guidance
- Suggested remediation

See the ai directory for the incident-analysis implementation.

## Documentation

- docs/architecture.md
- docs/implementation.md
- docs/deployment.md
- docs/troubleshooting.md

## Project Structure

- ai/ - AI-assisted incident analysis
- ansible/ - server configuration and deployment
- docs/ - project documentation
- helm/ - Helm chart
- kubernetes/ - Kubernetes manifests
- logging/ - ELK configuration
- monitoring/ - Prometheus and Grafana configuration
- scripts/ - Bash automation
- security/ - security controls and evidence
- terraform/ - AWS infrastructure as code
- Dockerfile - Nexvion container image
- compose.yaml - local container deployment
- Jenkinsfile - CI/CD pipeline

## Final Result

The project demonstrates an end-to-end DevOps delivery lifecycle around Nexvion using source control, automation, containers, CI/CD, infrastructure as code, configuration management, Kubernetes, monitoring, centralized logging, security, AI-assisted incident analysis and AWS cloud deployment.

---

## 🎬 Nexvion Project Demo

This screen recording demonstrates the Nexvion e-commerce
application, including the homepage and product catalogue.

### ▶ Watch Project Demo

[▶ Click here to watch the Nexvion demo](demo/Nexvion_Project_Demo_GitHub.mp4)

