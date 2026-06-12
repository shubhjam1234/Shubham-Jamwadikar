# Terraform + Terragrunt AWS Infrastructure

## 🚀 Overview

This repository demonstrates production-grade Infrastructure as Code (IaC) using **Terraform modules** and **Terragrunt live environments** to provision and manage AWS infrastructure across multiple environments.

It is designed following real-world DevOps practices used in scalable cloud environments.

---

## 🧱 Architecture

This project follows a **modular + environment-based approach**:

- **Terraform Modules** → Reusable infrastructure components
- **Terragrunt Live Environments** → Environment-specific configurations (dev / test / prod)

---

## 📦 Modules

| Module | Purpose |
|--------|--------|
| VPC    | Networking layer (subnets, routing, gateways) |
| EC2    | Compute instances provisioning |
| EKS    | Kubernetes cluster setup on AWS |

---

## 🌍 Environments

Each environment is isolated using Terragrunt:
