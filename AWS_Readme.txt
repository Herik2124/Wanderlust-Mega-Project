# AWS Configuration Summary

Region: ap-south-1
Cluster: wanderlust-eks (created via eksctl)
Instance Types: m7i-flex.large (EC2 for Jenkins, EKS nodes)
Security Groups: Custom rules for ports 22, 8080, 9000, 31576, 31000, 31100, etc.
IAM Roles: AdminAccess for cluster management
Storage: 30 GB gp3 per node
Monitoring: Prometheus & Grafana deployed via Helm on EKS

All provisioning done via Terraform scripts in /terraform and manifests in /kubernetes.
