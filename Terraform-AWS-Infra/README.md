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
```
terragrunt/live/
├── dev
├── test
└── prod
```

Each environment contains:
- VPC configuration
- EC2 provisioning
- EKS cluster setup

---

## ⚙️ Tech Stack

- Terraform
- Terragrunt
- AWS (VPC, EC2, EKS)
- Linux-based infrastructure
- Git for version control

---

## 🧠 Key Features

- Modular Terraform design (reusable infrastructure)
- Environment separation (dev / test / prod)
- Centralized configuration using Terragrunt
- Scalable AWS infrastructure provisioning
- Reduced duplication using DRY principles
- Production-style structure similar to enterprise setups

---

## 📁 Folder Structure
```
modules/
├── vpc
├── ec2
└── eks

terragrunt/live/
├── dev
├── test
└── prod
```

---

## 🚀 How to Deploy

### 1. Navigate to environment
```bash
cd terragrunt/live/dev/vpc
terragrunt init
terragrunt plan
terragrunt apply
