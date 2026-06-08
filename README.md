# Azure Key Vault Secret Manager

This repository contains the target configuration and SRE runtime files compiled by the **Azure Key Vault Secret Manager** dashboard module.

## 🚀 Description
Manage cloud credentials securely. Generate Key Vault policies configurations, certificate rotation schedulers, and dynamic secrets retrieval scripts.

## 🛠️ Specification Matrix
- **Primary Configuration File**: `/infra/keyvault/keyvault.tf`
- **Execution Command**: `terraform init && terraform apply -auto-approve`
- **Validation Command**: `terraform show`

## 📋 How to Run & Validate

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Pradeeptalari14/tp-azure-key-vault.git
   cd tp-azure-key-vault
   ```

2. **Run Execution Target:**
   ```bash
   terraform init && terraform apply -auto-approve
   ```

3. **Verify Runtime Stability:**
   ```bash
   terraform show
   ```

## 🔐 Security & Best Practices
* **Secret Isolation**: Use organization-level secrets (or SSM parameter hooks) rather than hardcoded environment variables inside files.
* **Pull Request Lifecycles**: Protect default branch merges with validation checks before merging code changes.
