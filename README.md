# practice-repo

This repository contains a ready-to-use Terraform project to deploy an Azure web application and common dependencies: Resource Group, Storage Account (with container), App Service Plan, Web App, Managed Identity, Key Vault, Azure SQL Server + Database, Application Insights, Log Analytics Workspace, and RBAC role assignments.

# Azure Terraform Web App Project

This repo provisions an Azure Web App with supporting infrastructure using Terraform.


## Quick start

1. Copy `terraform.tfvars.example` to `terraform.tfvars` and fill values.
2. `terraform init`
3. `terraform plan -out plan.tfplan`
4. `terraform apply plan.tfplan`

## Notes
- Secrets are created in Key Vault.
- A user-assigned managed identity is attached to the Web App and given `Contributor` access to the storage account (example).
