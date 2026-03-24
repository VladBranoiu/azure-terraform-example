# Azure Terraform Example – Declarative Infrastructure Provisioning

This project demonstrates how to create Azure resources using **Terraform**, a popular Infrastructure-as-Code (IaC) tool.

Instead of manually creating resources in the Azure Portal, Terraform allows you to define infrastructure in code and deploy it in a consistent, repeatable way.

---

## 📌 What This Project Does

This Terraform configuration creates:

- A **Resource Group**
- A **Storage Account** inside that Resource Group

It is a simple example, but it introduces the core Terraform workflow and shows how Azure infrastructure can be provisioned declaratively.

---

## 🧠 Key Concept: Infrastructure as Code

Terraform lets you describe the infrastructure you want, such as:

- resource groups
- storage accounts
- virtual machines
- databases

Then Terraform compares your configuration with the actual state in Azure and applies the required changes.

This makes deployments:

- repeatable
- version-controlled
- easier to maintain
- less error-prone than manual setup

---

## 🏗️ Resources Created

### 1. Resource Group

```hcl
resource "azurerm_resource_group" "example" {
  name     = "my-terraform-rg"
  location = "France Central"
}
