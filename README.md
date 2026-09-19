# multi-cloud-devsecops-pipeline
 Multi-cloud production deployment pipeline featuring automated Syft/Grype supply chain security scanning and Checkov IaC linting for hardened AWS and Azure infrastructure.
# Multi-Cloud DevSecOps Pipeline with Automated Supply Chain Defense

## 🎯 Project Overview
This repository contains a production-grade, hardened CI/CD pipeline built to enforce a **"Shift Left" security posture** across multi-cloud environments. The pipeline validates source code, inventories software dependencies, checks for infrastructure drift, and safely deploys containerized web workloads to **AWS (EC2/ECR)** and **Azure (App Services)**.

## 🛡️ Threat Model & Security Controls
*   **Supply Chain Attacks:** Mitigation of malicious component injections (e.g., CVE-2024-3094 vectors) using automated **Syft** SBOM compilation and **Grype** vulnerability scanning.
*   **Infrastructure Misconfigurations:** Static analysis of Terraform templates via **Checkov** to prevent public exposure of cloud resources before provisioning.
*   **Credential Leakage:** Inclusion of GitGuardian scanning in pipeline runners to block hardcoded API keys and cloud secrets.

## 🛠️ Tech Stack & Lab Components
*   **CI/CD Engine:** GitHub Actions / YAML Workflows
*   **Cloud Architecture:** AWS (ECR, EC2, VPC) | Azure (App Services, Container Registry)
*   **DevSecOps Tools:** Syft (CycloneDX 1.5 JSON), Grype, Checkov, Terraform
