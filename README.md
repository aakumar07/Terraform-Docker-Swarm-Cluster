

# Terraform Docker Swarm Cluster Deployment

This repository contains Terraform scripts to automate the deployment of a Docker Swarm cluster on AWS EC2 instances. Docker Swarm allows you to manage a cluster of Docker engines, providing native clustering capabilities to turn a group of Docker engines into a single virtual Docker engine.

## Prerequisites

Before you begin, ensure you have the following:

- AWS account with appropriate permissions.
- Terraform installed locally. See [Terraform Installation Guide](https://learn.hashicorp.com/tutorials/terraform/install-cli) for instructions.
- AWS CLI installed and configured with an IAM user's access key and secret key.

## Steps to Deploy

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/aakumar07/Terraform-Docker-Swarm-Cluster.git
   cd Terraform-Docker-Swarm-Cluster
   ```

2. **Update AWS Key Location and Name:**
   Replace the default key location and name in Terraform configuration files (`variables.tf`, `main.tf`) with your own key details.

3. **Validate Terraform Configuration:**
   ```bash
   terraform validate
   ```

4. **Plan Deployment:**
   ```bash
   terraform plan
   ```

5. **Apply Deployment:**
   ```bash
   terraform apply
   ```
   Enter `yes` when prompted to confirm the deployment.

6. **Accessing the Docker Swarm Cluster:**
   After deployment, follow Terraform output or AWS Console to access the Docker Swarm cluster.

## Customization

- Adjust `variables.tf` and `main.tf` to customize cluster size, instance types, and other parameters.

## Cleanup

To destroy the Docker Swarm cluster and associated resources:

```bash
terraform destroy
```

Enter `yes` when prompted to confirm destruction.

## Contributing

Contributions are welcome! Feel free to open issues or pull requests for any improvements or fixes.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
