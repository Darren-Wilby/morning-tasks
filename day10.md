# Terraform Enterprise Approaches

## 1. What is remote state in Terraform and why is it important for collaborative projects?

Remote state in Terraform refers to storing the state file containing the current state of your infrastructure in a shared location, usually outside of your local working directory. It is essential for collaboration because it enables multiple users to work on the same infrastructure.

## 2. What are some advantages to remote state besides being able to work collaboratively?

-   Concurrency control. Avoids conflicts by providing locking mechanisms to prevent simultaneous updates from different users.
-   State managemnent. Centralised state management allows accurate tracking of infrastructure changes and versions over time.
-   Security. Reduces the risk of exposing secrets or confidential information.

## 3. What are some options for remote backends and how do they differ?

​Amazon S3, Azure Blob Storage, HashiCorp Terraform Cloud.

## 4. Why is it important to not hardcode secrets, like API keys and passwords, directly into your Terraform config?

​This is a big security risk as anyone with access could see them.

## 5. Provide an example of where using multiple Terraform workspaces would be beneficial

Development, staging, production. One is your actual deployed infrastructure, others are for developing and testing.
