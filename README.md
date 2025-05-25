# Azure Terraform Infra Demo

这是一个用 Terraform 自动部署 Azure 基础架构的简单示例，包含以下内容：

- 资源组（Resource Group）
- 虚拟网络（VNet）
- 子网（Subnet）

---

## 📁 项目结构
azure-terraform-infra-demo/
├── main.tf # 主资源定义
├── variables.tf # 变量声明
├── terraform.tfvars # 变量赋值
├── outputs.tf # 输出值


---

## 🚀 使用方法

1. 登录 Azure CLI：
```bash
az login

2.初始化 Terraform：
terraform init

3.查看计划：
terraform plan

4.执行部署：
terraform apply

🧠 作者
Smallsun2025
专注 Azure IaaS × Terraform × 自动化部署。



