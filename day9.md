# Terraform

​

### 1. What is infrastructure as code (IaC) and why is it important in modern IT operations? What are the advantages?

Managing and provisioning infrastructure using code and automation. It allows you to configure servers using scripts rather than manually.
Advantages: automation, consistency, version control, reproducibility: You can easily recreate and rebuild environments with the same code, making testing and development more reliable, scalability, reduced errors, faster recovery.​
​

### 2. Explain the concept of "Infrastructure as Code" (IaC) and how Terraform fits into this concept.

​Terraform is a tool that allows you to create IaC, it can be used for AWS, Azure, and Google Cloud.

### 3. What problems do modules help address, and how do they promote reusability?

​They reduce code duplication and allows reusability.

### 4. Explain in your own words what the following commands achieve;

​

### - `terraform init`

Initializes a Terraform working directory, downloading and installing the required providers and modules.

### - `terraform plan`

Generates an execution plan detailing what Terraform will do when applying the configuration, including changes, additions, and deletions.

### - `terraform apply`

Applies the changes specified in the configuration, creating or updating resources to match the desired state.

### - `terraform destroy`

Destroys all resources created by the configuration, effectively tearing down the infrastructure.

### - `terraform fmt`

Formats the Terraform configuration files for consistent style and readability.

### - `terraform output`

Displays outputs defined in the configuration, which are useful for getting information about the created resources.

### - `terraform taint`

Marks a specific resource for recreation during the next terraform apply, allowing you to re-create a resource even if it hasn't changed in the configuration.
