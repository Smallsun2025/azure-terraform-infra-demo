Automate VM Image Creation on Azure with Terraform
📌 1. Introduction
Creating a reusable VM image is a core part of cloud infrastructure workflows. In this tutorial, we’ll use Terraform to create a Managed Image from an existing Azure VM — fully automated and reproducible. This is especially useful when building base images for application servers, golden images for dev/test, or setting up a repeatable environment base.

📁 2. Project Structure
The project contains the following Terraform files:

azure-managed-image/
├── main.tf # Define VM and image resources
├── variables.tf # Declare input variables
├── terraform.tfvars # Provide actual values for variables
├── outputs.tf # Output the Managed Image ID

⚙️ 3. What the Terraform Code Does

Provisions a temporary Virtual Machine using azurerm_windows_virtual_machine.
Adds a custom script (startup-script.sh) to configure the VM during creation.
After VM is ready, it creates a Managed Image from this VM.
Outputs the image ID, which can be used in future Terraform configurations.
🚀 4. How to Deploy

Make sure you have the Azure CLI installed and logged in (az login), and Terraform installed.

Then follow these commands:

terraform init

terraform plan

terraform apply

After a few minutes, you’ll get the Managed Image ID in the output.

✅ 5. Conclusion
By using Terraform to create a Managed Image, we can simplify our infrastructure pipeline and reuse golden images in future deployments. This is a core DevOps practice that helps ensure consistency and efficiency in cloud environments.

🔜 Coming Next:

Deploying VMs from Managed Images
Creating Image Versions with Shared Image Gallery
Using Packer + Terraform for advanced image pipelines
Thanks for reading! ⭐️ this repo if you found it helpful!
